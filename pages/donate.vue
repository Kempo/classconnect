<template>
  <div class="contianer">
    <div class="header">
      <center>Donate to Rainier Beach</center>
    </div>
    <hr style="width: 100%;" />
    <div class="school-details">
      <div class="about-school">
        <b-card no-body>
          <b-card-body>
            <b-card-title style="display:inline-block; height:2em">
              Rainier Beach High School
              <b-col md="3" style="float:right">
                <b-card-img
                  src="https://picsum.photos/400/400/?image=20"
                  class="rounded-0"
                ></b-card-img>
              </b-col>
            </b-card-title>
            <b-card-sub-title class="mb-2">
              Funding Goal: $1500
            </b-card-sub-title>
            <b-card-text>
              Grades K-12
            </b-card-text>
            <b-card-body>
              <a href="#" class="card-link">School Website</a>
              <a href="#" class="card-link">PTA Website</a>
            </b-card-body>
          </b-card-body>
          <b-list-group flush>
            <b-list-group-item>
              <div class="content">
                <div class="question">Number of Students:</div>
                <div class="res">225</div>
              </div>
            </b-list-group-item>
            <b-list-group-item>
              <div class="content">
                <div class="question">Free or Reduced Lunch:</div>
                <div class="res">78%</div>
              </div>
            </b-list-group-item>
            <b-list-group-item>
              <div class="content">
                <div class="question">Current PTA Budget:</div>
                <div class="res">$0.00</div>
              </div>
            </b-list-group-item>
            <b-list-group-item>
              <div class="content">
                <div class="question">Avg Teacher Salary:</div>
                <div class="res">$77,000/year</div>
              </div>
            </b-list-group-item>
            <b-list-group-item>
              <div class="content">
                <div class="question">Student Teacher Ratio:</div>
                <div class="res">15:1</div>
              </div>
            </b-list-group-item>
          </b-list-group>
          <b-card-body>
            <b-card-title>Name of Tier 1</b-card-title>
            <b-card-sub-title class="mb-2">
              Tier 1
            </b-card-sub-title>
            <b-card-text>
              Here are all the things they want from tier one
              <div class="progress">
                <div
                  class="progress-bar progress-bar-warning progress-bar"
                  role="progressbar"
                  aria-valuenow="70"
                  aria-valuemin="0"
                  aria-valuemax="100"
                  style="width:100%"
                >
                  Completed: Raised $400 of 400
                </div>
              </div>
            </b-card-text>
          </b-card-body>
          <b-card-body>
            <b-card-title>Name of Tier 2</b-card-title>
            <b-card-sub-title class="mb-2">
              Tier 2
            </b-card-sub-title>
            <b-card-text>
              Here are all the things they want from tier two
              <div class="progress">
                <div
                  class="progress-bar progress-bar-warning progress-bar-striped"
                  role="progressbar"
                  aria-valuenow="70"
                  aria-valuemin="0"
                  aria-valuemax="100"
                  style="width:70%"
                >
                  Raised $700 of $1000
                </div>
              </div>
            </b-card-text>
          </b-card-body>
          <b-card-body>
            <b-card-title>Name of Tier 3</b-card-title>
            <b-card-sub-title class="mb-2">
              Tier 3
            </b-card-sub-title>
            <b-card-text>
              Here is everything they want from tier 3
              <div class="progress">
                <div
                  class="progress-bar empty-bar"
                  role="progressbar"
                  aria-valuenow="0"
                  aria-valuemin="0"
                  aria-valuemax="100"
                  style="width:100%"
                >
                  Not Started
                </div>
              </div>
            </b-card-text>
          </b-card-body>
        </b-card>
      </div>
    </div>
    <div class="left-container">
      <b-card no-body class="message">
        <b-card-body>
          <b-card-title>Message from the PTA</b-card-title>
          <b-card-text>
            Hi, this is Pamela from RBHS PTA! Right now to support our history
            and writing classes, we are down stationery supplies for 5 classes.
            Please help us out! Thank you :)
          </b-card-text>
        </b-card-body>
      </b-card>
      <br />
      <br />
      <div class="select-donation">
        <center><strong>Select Your Donation</strong></center>
        <br />
        <center>
          <div class="donation-amt">
            <button class="amount btn btn-primary">$5</button>
            <button class="amount btn btn-primary">$10</button>
            <button class="amount btn btn-primary">$15</button>
            <br />
            <br />
            <form>
              <label>
                $
                <input type="text" placeholder="100" class="input-text" />
              </label>
            </form>
          </div>
        </center>
      </div>
    </div>
  </div>
</template>

<script></script>

<style>
@import url('https://fonts.googleapis.com/css?family=Poppins&display=swap');
.header {
  font-size: 3em;
  margin-bottom: 0.4em;
  margin-top: 0.2em;
}
hr {
  width: 80%;
  align: center;
}
.select-donation {
  position: fixed;
  background-color: #ccc;
  margin-bottom: 0;
  padding: 1.75em;
  width: 35%;
  border-radius: 5px;
}

.donation-amt {
  display: table-row;
  float: right;
  width: 100%;
}
.about-school {
  display: flex;
  flex-direction: column;
  padding-left: 2em;
}

button {
  margin: 0.1em;
  width: 25%;
  display: table-cell;
}
input[type='text'] {
  margin: 0.5em;
}
.container {
  display: flex;
}
.school-details {
  float: left;
  width: 57%;
  margin-bottom: 2em;
}

input {
  border: none;
  background: #eee;
}
label {
  color: #777;
  display: table-cell;
  background: #eee;
  border-radius: 5px;
  margin: 0.5em;
  padding-left: 0.7em;
  margin-left: 2em;
}
button:nth-child(3) {
  margin-right: 0.25em;
}

.progress {
  height: 30px;
}
.empty-bar {
  background-color: #e9ecef;
  color: #000;
}
.left-container {
  width: 35%;
  float: right;
  margin-right: 2em;
}
.content {
  display: inline-blok;
  width: 100%;
}
.question {
  float: left;
  font-weight: bolder;
}
.res {
  float: right;
  padding-righ: 2em;
}
b-card-title {
  height: 1em;
}
</style>
