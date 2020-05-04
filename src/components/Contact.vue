<template>
  <section id="contact" class="page-footer">
    <div class="container">
        <div class="content-bg text-center avatar-section">
        <h1 class="contact__title text-center">Contact Me</h1>
        <div class="contact__content">
          <hr class="contact__content--line">
          <div class="text-center contact__content--links">
              <a href="https://ca.linkedin.com/in/shabnamkimiai" class="contact-icon">
               <font-awesome-icon :icon="[ 'fab', 'linkedin' ]" style="color: #444" size="3x" />
              </a>
              <a href="https://github.com/shab-k" class="contact-icon">
                <!-- <i class="fab fa-github-square fa-3x" style="color:#d2d0d8"></i> -->
                <font-awesome-icon :icon="[ 'fab', 'github' ]" style="color: #444" size="3x" />
              </a>
              <a type="button" class="btn contact-icon" data-toggle="tooltip" data-placement="bottom"
                title="shab.k.web [at] gmail">
                   <!-- <i class="fas fa-envelope-square fa-3x" style="color:#444"></i> -->
                   <font-awesome-icon :icon="[ 'fas', 'envelope' ]" style="color: #444" size="3x" />
              </a>
        </div>
         <hr class="contact__content--line">
        </div>
      </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Contact'
}
</script>
