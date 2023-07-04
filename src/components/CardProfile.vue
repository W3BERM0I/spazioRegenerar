<template>
  <v-card class="elevation-10 rounded-xl cardProfile">
    <v-row style="position: relative" class="justify-center align-center">
      <v-sheet
        style="position: absolute"
        :color="profile.color"
        cover
        height="200"
        class="rounded sheetProfile"
      >
      </v-sheet>
      <v-avatar class="imgProfile" size="140" :image="profile.imgSrc">
      </v-avatar>
    </v-row>
    <v-row class="nameDescription">
      <v-list-item
        :title="profile.name"
        :subtitle="profile.description"
      ></v-list-item>
    </v-row>

    <v-row class="d-flex align-center justify-space-around ma-4">
      <a :href="profile.whats" target="_blank" rel="noopener noreferrer">
        <v-icon size="40" style="color: green">mdi-whatsapp</v-icon>
      </a>
      <a :href="profile.insta" target="_blank" rel="noopener noreferrer">
        <v-icon size="40" class="insta">mdi-instagram</v-icon>
      </a>
    </v-row>
  </v-card>
</template>

<script setup>
const props = defineProps({ profile: Object });
</script>

<style>
.cardProfile {
  width: 400px;
  min-height: 450px;
  align-content: flex-end;
  justify-content: flex-end;
}

.sheetProfile {
  width: 100%;
}

.insta {
  color: #f09433;
  color: -moz-linear-gradient(
    45deg,
    #f09433 0%,
    #e6683c 25%,
    #dc2743 50%,
    #cc2366 75%,
    #bc1888 100%
  );
  color: -webkit-linear-gradient(
    45deg,
    #f09433 0%,
    #e6683c 25%,
    #dc2743 50%,
    #cc2366 75%,
    #bc1888 100%
  );
  color: linear-gradient(
    45deg,
    #f09433 0%,
    #e6683c 25%,
    #dc2743 50%,
    #cc2366 75%,
    #bc1888 100%
  );
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f09433', endColorstr='#bc1888',GradientType=1 );
}

.imgProfile {
  position: absolute;
  z-index: 1;
  top: 70px;
}

.nameDescription {
  margin-top: 100px;
  padding: 10px;
  min-height: 300px;
}

.v-list-item {
  justify-content: center !important;
  align-items: center;
  margin-top: 80px;
}

.v-list-item-title,
.v-list-item-subtitle {
  font-size: 1.6rem !important;
  line-height: 1.5rem !important;
  margin-bottom: 10px;
  align-items: center;
}
</style>