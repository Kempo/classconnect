<template>
  <div>
    <center style="margin-bottom: 0.4em; margin-top: 0.2em;">
      <h1 style="font-size: 3em;">Explore local schools</h1>
    </center>
    <hr />
    <div
      style="padding: 50px 50px 0px 50px; display: flex; flex-direction: column;"
    >
      <b-card
        v-for="a in assocs"
        :key="a.name"
        :header="a.name"
        style="width: 70%; max-width: 800px; margin: 25px;"
      >
        <b-row no-gutters>
          <b-col md="3" style="margin-right: 25px;">
            <b-card-img
              src="https://picsum.photos/400/400/?image=20"
              width="200"
            ></b-card-img>
          </b-col>
          <b-col>
            <b-card-title>{{ a.name }}</b-card-title>
            <b-card-sub-title>{{ a.address }}</b-card-sub-title>
            <hr />
            <b-card-text>
              {{ a.tiers[a.current].desc }}
            </b-card-text>

            <b-card-text
              >Current Tier: <strong>#{{ a.current + 1 }}</strong>
              {{ a.tiers[a.current].name }}
            </b-card-text>

            <b-card-sub-title>
              <strong>{{ a.tiers[a.current].deal }}</strong>
            </b-card-sub-title>
          </b-col>
        </b-row>
        <br />
        <div>
          <b-progress :max="a.tiers[a.current].goal" height="30px">
            <b-progress-bar :value="a.tiers[a.current].raised">
              <p style="margin-top: 15px;">
                Raised: $<strong>{{ a.tiers[a.current].raised }}</strong> of
                <strong>${{ a.tiers[a.current].goal }}</strong>
              </p>
            </b-progress-bar>
          </b-progress>
          <br />
          <b-button href="/donate" variant="danger">Donate</b-button>
        </div>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      assocs: [
        {
          name: 'Rainier Beach High School',
          address: '8815 Seward Park Ave S, Seattle, WA 98118',
          current: 2,
          tiers: [
            {
              name: 'Computer Science Textbooks',
              goal: 1000,
              raised: 600
            },
            {
              name: 'Whiteboards',
              goal: 500,
              raised: 400
            },
            {
              name: 'Stationery (pencils, erasers, highlighters)',
              goal: 500,
              raised: 300,
              deal: "Donate now to receive 25% off at Sherry's Italian!",
              desc:
                'Hi, this is Pamela from RBHS PTA! Right now to support our history and writing classes, we are down stationery supplies for 5 classes. Please help us out! Thank you :)'
            }
          ]
        },
        {
          name: 'Garfield High School',
          address: '400 23rd Ave, Seattle, WA 98122',
          current: 0,
          tiers: [
            {
              name: 'Classroom Projectors',
              goal: 1000,
              raised: 700,
              deal: 'Microsoft is currently matching every donation!',
              desc:
                "Hello! This is Angela. I'm the current leader for Garfield PTA. We are in dire need of classroom projectors for our Language Arts and Film classes. Any amount is helpful!"
            },
            {
              name: 'Pencils',
              goal: 1000,
              raised: 400
            },
            {
              name: 'Pencils',

              goal: 1000,
              raised: 400
            }
          ]
        },
        {
          name: 'Franklin High School',
          address: '3013 S Mt Baker Blvd, Seattle, WA 98144',
          current: 0,
          tiers: [
            {
              name: 'Desks and Chairs',
              goal: 1000,
              raised: 400,
              deal: "Receive 10% at Ezell's Fried Chicken",
              desc:
                'Hi, this is Pamela from RHS PTSA! Right now to support our history and writing classes, we are down stationery supplies for 5 classes. Please help us out! Thank you :)'
            },
            {
              name: 'Pencils',
              goal: 1000,
              raised: 400
            },
            {
              name: 'Pencils',
              goal: 1000,
              raised: 400
            }
          ]
        }
      ]
    }
  }
}
</script>

<style></style>
