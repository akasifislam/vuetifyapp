<template>
  <v-container class="my-15">
      <v-row justify="center">
          <v-col lg="12" class="text-center">
              <v-subheader class="text-h4 justify-center">Contact Us</v-subheader>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis ut dolore laudantium nulla eveniet alias minus explicabo ea labore vitae quod cupiditate et doloremque repellat quam, iure expedita consequatur quo</p>
          </v-col>
          <v-col lg="6">
              <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d58894.13647543677!2d90.31878474254528!3d22.695379290521466!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x37553407fbece487%3A0x5d069b9599d4414a!2sBarishal!5e0!3m2!1sen!2sbd!4v1634913524821!5m2!1sen!2sbd" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
          </v-col>
          <v-col lg="6">
              <v-form
                    ref="form"
                >
                    <v-text-field
                    v-model="contactInfo.name"
                    :counter="10"
                    label="Name"
                    required
                    ></v-text-field>

                    <v-text-field
                    v-model="contactInfo.email"
                    label="E-mail"
                    required
                    ></v-text-field>
                    <v-textarea label="Massage" v-model="contactInfo.Massage">

                    </v-textarea>
                    <v-btn
                    color="success"
                    class="mr-4"
                    >
                    Send
                    </v-btn>
                </v-form>
          </v-col>
        </v-row>
    </v-container>
  
</template>

<script>
export default {
    data() {
        return {
            contactInfo: {}
        }
    }
} 
</script>

<style>

</style>