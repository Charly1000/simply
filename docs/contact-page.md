# Contact Page

- Create a new page
- Choose your favorite URL and title
- Select the `Archive Contact` template from the Template drop down
- Publish the page
- To add the page to the navigation

➡️ Add your content and the contact form code using [FORMSPREE](https://formspree.io/) as a service. Please check the code example below.

```html
<form
  action="https://formspree.io/your@email.com"
  class="mt-10 grid md:grid-cols-2 gap-6"
  method="POST">

  <input name="name" class="col-span-1" type="text" placeholder="Your Name" required>
  <input name="email" class="col-span-1" type="email" placeholder="Your Email" required>
  <textarea name="message" class="col-span-full" placeholder="Type Message" required></textarea>
  <div class="col-span-full text-center"><button type="submit" class="button is-primary">Send Message</button></div>
</form>
```

![Ghost - Simply Contact Page](https://user-images.githubusercontent.com/10253167/162016633-7d328cc5-d5de-407a-bf03-57439985c024.jpg)


for example, you can add following to create clickable contact. E-Mail address isn't in plaintext, it's encrypted with javascript. So it's not so good for bots but better for you :)

```html
<div class="grid md:grid-cols-3 gap-6 text-center mt-20 kg-width-wide text-base">
    <div class="flex flex-col items-center">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <rect x="5" y="2" width="14" height="20" rx="2" ry="2"></rect>
          <line x1="12" y1="18" x2="12" y2="18"></line>
      </svg>
        <h4 class="my-5 text-lg">PHONE</h4>
        <p><a href="tel:+1234567890" target="_blank">+1 234 567890</a> (click)</p>
          <p><a href="https://wa.me/1234567890" target="_blank"><i class="fa fa-whatsapp fa_custom"></i><font color="#00BB00"> WhatsApp</font></a> (click)</p>
          <p><a href="https://teams.microsoft.com/l/chat/0/0?users=YOUREMAILADRESS&topicname=Chat" target="_blank">Chat with Microsoft Teams</a> (click)</p>
    </div>
    <div class="flex flex-col items-center">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"></path>
          <circle cx="12" cy="10" r="3"></circle>
      </svg>
        <h4 class="my-5 text-lg">ADRESS</h4>
            <p>STREET NO, EX LOC WHERE YOU LIVE, COUNTRY</p>
    </div>
    <div class="flex flex-col items-center">
        <svg viewBox="0 0 24 24" width="64" height="64" stroke="currentColor" stroke-width="1" fill="none" stroke-linecap="round" stroke-linejoin="round">
          <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
          <polyline points="22,6 12,13 2,6"></polyline>
      </svg>
        <h4 class="my-5 text-lg">EMAIL</h4>
        <p><SCRIPT TYPE="text/javascript">
emailE='YOUR TLD HERE'
emailE=('BEFORE AT SIGN' + '@' + emailE)
document.write('<A href="mailto:' + emailE + '">' + emailE + '</a>')
</script> (click)</p>
    </div>
</div>
```
