<template>
  <div
    id="bcregistries-account"
    class="account-container d-flex flex-column"
    style="padding-bottom: 70px; padding-top: 100px"
  >
    <v-container no-gutters style="padding-bottom: 30px">
      <div class="menu-title">BC Registries Account</div>
      <v-row>
        <v-col cols="2"></v-col>
        <v-col cols="8" class="menu-info"
          >As we work to modernize our digital registries services, features
          from other account types are gradually being moved to the new BC
          Registries account system.</v-col
        >
        <v-col cols="2"></v-col>
      </v-row>
      <v-row>
        <v-col cols="2"></v-col>
        <v-col cols="8" class="menu-info-bold"
          >The new BC Registries account supports the following services:</v-col
        >
        <v-col cols="2"></v-col>
      </v-row>

      <v-card
        flat
        class="d-md-flex flex-wrap"
        style="background-color: #f1f3f5; padding-top: 30px"
      >
        <v-card flat max-width="350px" class="mr-5 mb-7">
          <v-card-title class="menu-header">
            <span class="menu-item-title">BC Business Registry</span>
            <v-spacer></v-spacer>
          </v-card-title>
          <v-card-text class="menu-item">
            <p>
              Manage the incorporation, registration, and listing of businesses
              and organizations in BC. Here you are currently able to:
            </p>
            <ul>
              <li>
                <span class="menu-list-text"
                  >Incorporate or manage benefit companies</span
                >
              </li>
              <li>
                <span class="menu-list-text"
                  >Manage cooperative associations</span
                >
              </li>
            </ul>
            <p style="padding-top: 30px">
              <a
                :href="$config.businessURL"
                target="_blank"
                rel="noopener noreferrer"
              >
                Go to BC Business Registry
              </a>
              <v-icon class="pl-1" color="primary" dark dense
                >mdi-open-in-new</v-icon
              >
            </p>
          </v-card-text>
        </v-card>
        <v-card flat max-width="350px" class="mr-5 mb-7">
          <v-card-title class="menu-header">
            <v-row>
              <v-col cols="9">
                <span class="menu-item-title">Name Requests (Beta)</span>
              </v-col>
              <v-col cols="3">
                <v-row>
                  <v-col cols="auto" class="menu-title-badge">NEW</v-col>
                </v-row>
                <v-row>
                  <v-col cols="auto"></v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-card-title>
          <v-card-text class="menu-item">
            <p>
              A new way to research and request a name for your new or existing
              BC business. Here you will be able to:
            </p>
            <ul>
              <li>
                <span class="menu-list-text">Search for a business name</span>
              </li>
              <li>
                <span class="menu-list-text"
                  >Manage your existing name request</span
                >
              </li>
            </ul>
            <p style="padding-top: 30px">
              <a
                :href="$config.nameRequestURL"
                target="_blank"
                rel="noopener noreferrer"
              >
                Go to Name Request
              </a>
              <v-icon class="pl-1" color="primary" dark dense
                >mdi-open-in-new</v-icon
              >
            </p>
          </v-card-text>
        </v-card>
        <v-card flat max-width="350px" class="mr-5 mb-7">
          <v-card-title class="menu-header">
            <v-row>
              <v-col cols="7">
                <span class="menu-item-title">Wills Registry</span>
              </v-col>
              <v-col cols="5">
                <v-row>
                  <v-col cols="auto" class="menu-title-badge"
                    >COMING SOON</v-col
                  >
                </v-row>
                <v-row>
                  <v-col cols="auto"></v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-card-title>
          <v-card-text class="menu-item">
            <p>
              <span style="font-weight: bold">Coming soon</span> to BC
              Registries Account, Wills Registry allows solicitors, notaries,
              and title search companies to do the following:
            </p>
            <ul>
              <li><span class="menu-list-text">File a wills notice</span></li>
              <li>
                <span class="menu-list-text"
                  >Search for an existing wills notice</span
                >
              </li>
            </ul>
            <!-- p style="padding-top: 30px">
              <a
                :href="$config.willsURL"
                target="_blank"
                rel="noopener noreferrer"
              >
                Go to Wills Registry
              </a>
              <v-icon class="pl-1" color="primary" dark dense
                >mdi-open-in-new</v-icon
              >
            </p -->
          </v-card-text>
        </v-card>
      </v-card>

      <v-card
        flat
        class="d-md-flex flex-wrap"
        style="background-color: #f1f3f5; padding-top: 2px"
      >
        <v-card flat max-width="350px" class="mr-5">
          <v-card-title class="menu-header">
            <v-row>
              <v-col cols="9"
                ><span class="menu-item-title"
                  >Personal Property Registry</span
                ></v-col
              >
              <v-col cols="3">
                <v-row>
                  <v-col cols="auto" class="menu-title-badge">ALPHA</v-col>
                </v-row>
                <v-row>
                  <v-col cols="auto"></v-col>
                </v-row>
              </v-col>
            </v-row>
          </v-card-title>
          <v-card-text class="menu-item">
            <p>
              A private alpha release of the new Personal Property Registry is
              available to a select group of users. Current functionality
              includes:
            </p>
            <ul>
              <li><span class="menu-list-text">Registration Search</span></li>
              <li>
                <span class="menu-list-text">Download PDF search reports</span>
              </li>
            </ul>
            <p style="padding-top: 30px">
              <nuxt-link to="/ppr-marketing"
                >Go to Personal Property Registry</nuxt-link
              >
              <v-icon class="pl-1" color="primary" dark dense
                >mdi-open-in-new</v-icon
              >
            </p>
          </v-card-text>
        </v-card>
      </v-card>
    </v-container>
    <div class="payment">
      <v-row>
        <v-col cols="2"></v-col>
        <v-col cols="8" class="payment-info-bold"
          ><v-icon medium color="#38598a">mdi-currency-usd-circle</v-icon
          ><span style="padding-left: 10px"
            >Multiple payment types:</span
          ></v-col
        >
        <v-col cols="2"> </v-col>
      </v-row>
      <v-row>
        <v-col cols="3"></v-col>
        <v-col cols="6" class="payment-info" style="max-width: 850px"
          >The BC Registries Account supports multiple payment options depending
          on the account and transaction type, including credit card, online
          banking, BC OnLine, and pre-authorized debit (PAD).
        </v-col>
        <v-col cols="3"></v-col>
      </v-row>
      <v-card
        flat
        tile
        class="menu-card-button justify-center d-flex flex-wrap"
      >
        <v-card flat tile class="pr-3" style="background-color: #e2e8ee">
          <SbcSigninButton />
        </v-card>
        <v-card flat tile class="pl-3" style="background-color: #e2e8ee">
          <v-btn
            class="button-gold"
            style="height: 40px"
            :href="$config.regAccountCreateURL"
            >Create a BC Registries Account</v-btn
          >
        </v-card>
      </v-card>
    </div>
  </div>
</template>

<script>
import SbcSigninButton from '~/components/SbcSigninButton.vue'
export default {
  components: {
    SbcSigninButton,
  },
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/theme.scss';

a {
  color: $BCgovLink !important;
  font-size: 1rem;
  font-weight: bold;
  text-decoration: underline;
}
</style>
