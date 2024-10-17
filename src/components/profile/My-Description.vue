<template>
    <div class="px-6">
        <div class="intro">
            <p class="text-4xl">Hello!</p>
            <p class="text-4xl my-2">I'm Samuel</p>
        </div>
        <p class="text-justify text-sm my-5">
            <span>Software Developer</span>
            With over 3+ years of experience in crafting dynamic
            and engaging web applications.
        </p>
        <div class="flex items-center justify-start gap-5">
            <div class="border border-gray-600 flex items-center justify-center h-10 w-10 rounded-lg bg-gray-900  hover:bg-gray-950 hover:text-white hover:translate-y-2 hover:transition-transform cursor-pointer">
                <i class="bi bi-linkedin text-xl"></i>
            </div>
            <div class="border border-gray-600 flex items-center justify-center h-10 w-10 rounded-lg bg-gray-900  hover:bg-gray-950 hover:text-white hover:translate-y-2 hover:transition-transform cursor-pointer">
                <i class="bi bi-github text-xl"></i>
            </div>
            
            <div>
                <button @click="openContactModal" class="border-2 border-gray-800 py-2 px-5 rounded-lg bg-white text-gray-900 hover:bg-gray-950 hover:text-white hover:translate-y-2 hover:transition-transform">
                    LET'S TALK
                </button>
            </div>
        </div>
        <button @click="downloadResume" class="border-2 my-5 border-gray-800 py-2 px-5 rounded-lg bg-gray-900 text-gray-200 hover:bg-gray-950 hover:text-white hover:translate-y-2 hover:transition-transform">
            <i class="bi bi-file-earmark-arrow-down-fill text-xl mr-3"></i> RESUME
        </button>
    </div> 
</template>

<script>
import Swal from 'sweetalert2';
export default {
    methods: {
        downloadResume() {
            const link = document.createElement('a');
            link.href = '/pdf/resume.pdf'; // Correct path relative to 'public'
            link.download = 'resume.pdf';
            document.body.appendChild(link); // Append the link to the document body
            link.click(); // Programmatically click the link
            document.body.removeChild(link); // Remove the link after the download
        },
        openContactModal() {
      Swal.fire({
        title: 'Contact Me',
        html: `
          <form id="contact-form" class="flex flex-col">
            <label for="email" class="text-sm font-semibold">Email:</label>
            <input type="email" id="email" name="email" class="w-full p-2 my-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-gray-400" placeholder="Enter your email" required />
            
            <label for="message" class="text-sm font-semibold">Message:</label>
            <textarea id="message" name="message" rows="4" class="w-full p-2 my-2 border border-gray-300 rounded focus:outline-none focus:ring-2 focus:ring-gray-400" placeholder="Enter your message" required></textarea>
            
            <button type="submit" class="w-full bg-gray-900 text-white py-2 mt-4 rounded-lg hover:bg-gray-700">Send Message</button>
          </form>
        `,
        showConfirmButton: false, // Hide default confirm button
        width: '600px', // Customize the width of the modal
        preConfirm: () => {
          const email = Swal.getPopup().querySelector('#email').value;
          const message = Swal.getPopup().querySelector('#message').value;

          if (!email || !message) {
            Swal.showValidationMessage('Please enter both email and message');
          }

          return { email, message };
        }
      }).then((result) => {
        if (result.value) {
          console.log('Email:', result.value.email);
          console.log('Message:', result.value.message);
          Swal.fire('Message Sent!', 'Thank you for reaching out.', 'success');
        }
      });
    }
    }
}
</script>

<style scoped>

</style>