<template>
  <div>
    <section class="cta">
      <b-container>
        <div class="row text-center">
          <div class="col-md-12 pt-5 pb-5">
            <h3>Want to have your validator name, logo, website url<br />
            and social links included in PolkaStats?</h3>
          </div>
        </div>
      </b-container>
    </section>
    <section>
      <b-container class="main pb-5 text-center">
        <h2 class="mt-4 mb-4">How to include your validator information in PolkaStats</h2>
        <b-alert variant="success" show>
          You will need both, <a href="https://keybase.io" target="_blank">Keybase</a> and <a href="https://github.com" target="_blank">GitHub</a> accounts in order to continue.<br />
          Make sure you have properly filled your full name, website, social links and have uploaded a profile picture in your Keybase profile.
        </b-alert>
        <b-card-group deck class="mt-4 mb-4">
          <b-card title="Step 1">
            <b-card-text>
              Login with your GitHub user and make a Fork of PolkaStats v2 repo: <a href="https://github.com/Colm3na/polkastats-v2" target="_blank">https://github.com/Colm3na/polkastats-v2</a>.
            </b-card-text>
          </b-card>
          <b-card title="Step 2">
            <b-card-text>
              Create a new folder named "stash_address_of_your_validator" inside <a href="https://github.com/Colm3na/polkastats-v2/tree/master/identities" target="_blank">identities folder</a>.
              In that folder place 3 new files with exactly this names, keybase_username with your <a href="https://keybase.io" target="_blank">Keybase</a> username on it. A logo.png (512x512 max) and <a href="https://raw.githubusercontent.com/derfredy/polkastats-v2/master/identities/DSpbbk6HKKyS78c4KDLSxCetqbwnsemv2iocVXwNe2FAvWC/validator_info.json" target="_blank">validator_info.json</a> following this schema. 
            </b-card-text>
          </b-card>
          <b-card title="Step 3">
            <b-card-text>
              Make a Pull Request to the master branch of the original repo: <a href="https://github.com/Colm3na/polkastats-v2" target="_blank">https://github.com/Colm3na/polkastats-v2</a>.
            </b-card-text>
          </b-card>
        </b-card-group>
        <h4 class="mt-4">Need help? Send me a message at <a target="_blank" href="mailto:polkastats@protonmail.com">polkastats@protonmail.com</a>.</h4>
      </b-container>
    </section>
  </div>
</template>
<script>
import axios from 'axios'
export default {
  head () {
    return {
      title: 'PolkaStats - For Kusama validators',
      meta: [
        { hid: 'description', name: 'description', content: 'Include your kusama validator info in PolkaStats' }
      ]
    }
  }
}
</script>
<style scoped>
.card-title {
  color: #ef1073;
}

/* Call to action */

.cta {
  color: #fff;
  background-color: #5bc0de;
  border-color: #14b6e6;
  background-image: linear-gradient(135deg, #670d35, #b1e2f1);
}

.cta h3 {
  line-height: 3rem;
}
</style>