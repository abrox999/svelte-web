<script>
  import { onMount } from "svelte";
  import Chart from "chart.js/auto/auto.js";

  function barChart() {
    var ctx = document.getElementById("myChart").getContext("2d");
    var myChart = new Chart(ctx, {
      type: "bar",
      data: {
        labels: [
          "SEP",
          "OCT",
          "NOV",
          "DEC",
          "JAN",
          "FEB",
          "MAR",
          "APR",
          "MAY",
          "JUN",
          "JUL",
          "AUG",
          "SEP",
        ],
        datasets: [
          {
            label: "Employees",
            data: [43, 49, 53, 57, 64, 69, 85, 88, 85, 85, 85, 87, 88],
            backgroundColor: ["rgba(75, 192, 192, 0.2)"],
            borderColor: ["rgba(75, 192, 192, 1)"],
            borderWidth: 1,
          },
        ],
      },
      options: {
        animation: {
          duration: 3000,
        },
        scales: {
          y: {
            beginAtZero: true,
          },
        },
      },
    });
  }
  onMount(barChart);
</script>

<input type="checkbox" id="sidebar-toggle" />
<div class="sidebar">
  <div class="sidebar-header">
    <h3 class="brand">
      <span class="material-symbols-outlined"> rocket_launch </span>
      <span>LOGO</span>
    </h3>
    <label for="sidebar-toggle" class="material-symbols-outlined"> menu </label>
  </div>
  <div class="sidebar-menu">
    <ul>
      <li>
        <a href="/">
          <span class="material-symbols-outlined">home</span>
          <span>Home</span>
        </a>
      </li>
      <li>
        <a href="/">
          <span class="material-symbols-outlined"> info </span>
          <span>My Info</span>
        </a>
      </li>
      <li>
        <a href="/">
          <span class="material-symbols-outlined"> person </span>
          <span>People</span>
        </a>
      </li>
      <li>
        <a href="/">
          <span class="material-symbols-outlined"> person_search </span>
          <span>Hiring</span>
        </a>
      </li>
      <li>
        <a href="/">
          <span class="material-symbols-outlined"> report </span>
          <span>Reports</span>
        </a>
      </li>
      <li>
        <a href="/">
          <span class="material-symbols-outlined"> folder </span>
          <span>Files</span>
        </a>
      </li>
    </ul>
  </div>
</div>

<div class="main-content">
  <header>
    <div class="search-wrapper">
      <span class="material-symbols-outlined"> search </span>
      <input type="search" placeholder="Search" />
    </div>
    <div class="social-icons">
      <span class="material-symbols-outlined"> notifications </span>
      <span class="material-symbols-outlined"> settings </span>
      <div />
    </div>
  </header>

  <main class="main">
    <h2 class="title">Overveiw</h2>
    <div class="dash-cards">
      <div class="card-single">
        <div class="card-body">
          <span class="material-symbols-outlined"> flight </span>
          <div>
            <h5>Vacation</h5>
            <h4>23 HOURS AVAILABLE</h4>
          </div>
          <span class="material-symbols-outlined"> sick </span>
          <div>
            <h5>Sick</h5>
            <h4>36 HOURS AVAILABLE</h4>
          </div>
        </div>
        <div class="card-footer">
          <a href="/">Request Time Off</a>
        </div>
      </div>
      <div class="card-single">
        <div class="card-body">
          <span class="material-symbols-outlined"> today </span>
          <div class="card-pic">
            <h5>Who's Out Today</h5>
            <div class="pic">
              <div class="img-1" />
              <div class="img-2" />
              <div class="img-3" />
            </div>
          </div>
        </div>
        <div class="card-footer">
          <a href="/">Full List</a>
        </div>
      </div>
      <div class="card-single">
        <div class="card-body">
          <span class="material-symbols-outlined"> inbox </span>
          <div>
            <h5>Inbox</h5>
            <h4>3 UNREAD MESSAGES</h4>
          </div>
          <span class="material-symbols-outlined"> task </span>
          <div>
            <h5>Tasks</h5>
            <h4>6 TASK AVAILABLE</h4>
          </div>
        </div>
        <div class="card-footer">
          <a href="/">Veiw All</a>
        </div>
      </div>
    </div>

    <section class="recent">
      <div class="activity-grid">
        <div class="activity-card">
          <h3>Announcements</h3>
          <div class="summary-single">
            <div class="img-4" />
            <div>
              <h5>
                Charlotte Abbott made a request: Compensation request for Amy
                Granger.
              </h5>
              <small>In 9 days</small>
            </div>
          </div>
          <hr />
          <div class="summary-single">
            <span class="material-symbols-outlined"> restaurant </span>
            <div>
              <h5>Lunch with employee for Dorothy Chou</h5>
              <small>Due Sep 3 (10 days ago)</small>
            </div>
          </div>
          <hr />
          <div class="summary-single">
            <span class="material-symbols-outlined"> chat </span>
            <div>
              <h5>Business card order</h5>
              <small>Unread</small>
            </div>
          </div>
          <hr />
          <div class="summary-single">
            <div class="img-5" />
            <div>
              <h5>Hello from David (Budget planing workshop)</h5>
              <small>15 min ago</small>
            </div>
          </div>
          <hr />
          <div class="summary-single">
            <span class="material-symbols-outlined"> account_circle </span>
            <div>
              <h5>
                Take a moment to select peers to give feedback about your team
                members.
              </h5>
              <small>
                Request for feedback must be sent before Sep 2 (11 days ago)
              </small>
            </div>
          </div>
          <hr />
          <div class="summary-single">
            <span class="material-symbols-outlined"> account_circle </span>
            <div>
              <h5>Danial Venace has provided feedback about Ryota Saito</h5>
              <small> 1 month ago </small>
            </div>
          </div>
        </div>

        <div class="summary">
          <div class="summary-card">
            <h4>Benifits</h4>
            <div class="summary-single">
              <span class="material-symbols-outlined"> monitor_heart </span>
              <div>
                <h5>Healt Insurance</h5>
                <small>Jan 25.2021 - Jan 24.2022</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> mood </span>
              <div>
                <h5>Dental Insurance</h5>
                <small>Jan 25.2021 - Jan 24.2022</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> savings </span>
              <div>
                <h5>401(K)</h5>
                <small>Jan 25.2020</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> health_and_safety </span>
              <div>
                <h5>Life Insurance</h5>
                <small>Jan 25.2020</small>
              </div>
            </div>
            <div class="card-footer">
              <a href="/">Veiw All</a>
            </div>
          </div>

          <div class="bday-card">
            <h4>Celebrations</h4>
            <div class="bday-flex">
              <div class="bday-img" />
              <div class="bday-info">
                <h5>Mike Wazowski</h5>
                <small>Birthday Today</small>
              </div>
            </div>
            <div class="text-center">
              <button>
                <span class="material-symbols-outlined"> celebration </span>
                Send Wishes
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="recent">
      <div class="activity-grid2">
        <div class="summary">
          <div class="summary-card">
            <h4>Training</h4>
            <div class="summary-single">
              <span class="material-symbols-outlined"> event </span>
              <div>
                <h5>Unlawful Harassment</h5>
                <small>Due Aug 16, 2022</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> event_available </span>
              <div>
                <h5>Getting Started With BambooHR</h5>
                <small>Due Jul 2, 2018</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> event_available </span>
              <div>
                <h5>Working from home during COVID-19</h5>
                <small>Due Jun 28, 2018</small>
              </div>
            </div>
            <div class="summary-single">
              <span class="material-symbols-outlined"> event_available </span>
              <div>
                <h5>BambooHR Advantage Pakage Demo Video</h5>
                <small>Product Traning</small>
              </div>
            </div>
          </div>

          <div class="bday-card">
            <h4>Company Links</h4>
            <hr />
            <div class="summary-single">
              <div>
                <h5>Company</h5>
                <small>Company Website</small>
              </div>
            </div>
            <hr />
            <div class="summary-single">
              <div>
                <h5>Benifits</h5>
                <small>Vision</small><br />
                <small>Health</small><br />
                <small>Dental</small><br />
                <small>401K</small>
              </div>
            </div>
            <hr />
            <div class="summary-single">
              <div>
                <h5>COVID-19</h5>
                <small>COVID-19 CDC Fact Sheet</small><br />
                <small>CDC Overveiw of COVID-19</small>
              </div>
            </div>
          </div>
        </div>
        <div class="activity-card">
          <h3>Report</h3>
          <canvas id="myChart" />
        </div>
      </div>
    </section>
    <hr />
    <footer class="copyright">
      Privacy Policy - Terms of Service - © 2015-2022 Company name All rights
      reserve.
    </footer>
  </main>
</div>

<style>
  #sidebar-toggle {
    display: none;
  }
  #sidebar-toggle:checked ~ .sidebar {
    width: 60px;
  }
  #sidebar-toggle:checked ~ .sidebar .sidebar-header h3 span,
  #sidebar-toggle:checked ~ .sidebar li span:last-child {
    display: none;
  }
  #sidebar-toggle:checked ~ .sidebar .sidebar-header,
  #sidebar-toggle:checked ~ .sidebar li {
    display: flex;
    justify-content: center;
  }

  #sidebar-toggle:checked ~ .main-content {
    margin-left: 60px;
  }
  #sidebar-toggle:checked ~ .main-content header {
    left: 60px;
    width: calc(100% - 60px);
  }
  .sidebar {
    height: 100%;
    width: 240px;
    position: fixed;
    left: 0;
    top: 0;
    z-index: 100;
    background: var(--main-color);
    color: #efefef;
    overflow-y: auto;
    transition: width 500ms;
  }
  .sidebar-header {
    display: flex;
    align-items: center;
    height: 60px;
    padding: 0rem 1rem;
    justify-content: space-between;
  }
  .sidebar-menu {
    padding: 1rem;
    padding-top: 2rem;
  }

  .sidebar li {
    margin-bottom: 1.5rem;
  }

  .sidebar a {
    color: #fff;
    font-size: 18px;
  }
  .material-symbols-outlined {
    font-size: 19px;
  }
  .sidebar a span:last-child {
    padding-left: 0.6rem;
  }
  .main-content {
    position: relative;
    margin-left: 240px;
    transition: margin-left 500ms;
  }
  header {
    position: fixed;
    left: 240px;
    top: 0;
    z-index: 100;
    width: calc(100% - 240px);
    background: #fff;
    height: 60px;
    padding: 0rem 1rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid #ccc;
    transition: left 500ms;
  }
  .search-wrapper {
    display: flex;
    align-items: center;
  }
  .search-wrapper input {
    border: 0;
    outline: 0;
    padding: 1rem;
    height: 38px;
  }
  .social-icons {
    display: flex;
    align-items: center;
  }
  .social-icons span,
  .social-icons div {
    margin-left: 1.2rem;
  }
  .social-icons div {
    height: 38px;
    width: 38px;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("https://www.pngkit.com/png/full/433-4336764_john-cena-new-2018-png-by-ambriegnsasylum16-john.png");
    border-radius: 50%;
  }
  main {
    margin-top: 60px;
    background: #f1f5f9;
    min-height: 90vh;
    padding: 1rem 3rem;
  }
  .title {
    color: var(--color-dark);
    margin-bottom: 1rem;
  }

  .dash-cards {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-column-gap: 3rem;
  }
  .card-single {
    background: #fff;
    border-radius: 7px;
    box-shadow: 2px 2px 2px rgba(0, 0, 0, 0.2);
  }
  .card-body {
    padding: 1.3rem 1rem 2rem;
    display: flex;
    align-items: center;
  }
  .card-body span {
    font-size: 2rem;
    color: #777;
    padding-right: 1.4rem;
  }
  .card-body h5 {
    color: var(--text-grey);
    font-size: 1.5rem;
  }
  .card-body h4 {
    color: var(--color-dark);
    font-size: 1.1rem;
    margin-top: 0.4rem;
  }
  .card-footer {
    padding: 0.5rem 1rem;
    background: #f9fafc;
  }
  .card-footer a {
    color: var(--main-color);
  }

  .card-pic {
    align-items: center;
  }

  .img-1,
  .img-2,
  .img-3 {
    height: 45px;
    width: 45px;
    border-radius: 50%;
    display: inline-block;
    border: 3px solid #efefef;
    background-size: cover;
    background-repeat: no-repeat;
  }

  .img-1 {
    background-image: url("data:image/jpeg;base64,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");
  }
  .img-2 {
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQwir5RMScrpURSYwWIHxDwTubgGew2k-VQag&usqp=CAU");
  }
  .img-3 {
    background-image: url("data:image/png;base64,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");
  }
  .img-4 {
    height: 60px;
    width: 60px;
    border-radius: 50%;
    border: 3px solid #efefef;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTRf8JQ03uImWos_jnR9cRqivwYsP8q6bWbAg&usqp=CAU");
    margin-right: 0.8rem;
  }
  .img-5 {
    height: 60px;
    width: 60px;
    border-radius: 50%;
    border: 3px solid #efefef;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSg4EJLd7DrHH6IoYDrLXJ5kgdxiwiMkk8OJw&usqp=CAU");
    margin-right: 0.8rem;
  }

  .recent {
    margin-top: 3rem;
    margin-bottom: 3rem;
  }
  .activity-grid {
    display: grid;
    grid-template-columns: 75% 25%;
    grid-column-gap: 1.5rem;
  }
  .activity-grid2 {
    display: grid;
    grid-template-columns: 25% 75%;
    grid-column-gap: 1.5rem;
  }
  .activity-card,
  .summary-card,
  .bday-card {
    background: #fff;
    border-radius: 7px;
  }
  .activity-card h3 {
    color: var(--text-grey);
    margin: 1rem;
  }
  .summary-card {
    margin-bottom: 1.5rem;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
  .summary-card h4 {
    padding: 0.5rem 1rem;
    color: var(--text-grey);
    font-size: 1.5rem;
  }

  .summary-single {
    padding: 0.5rem 1rem;
    display: flex;
    align-items: center;
  }
  .summary-single span {
    font-size: 1.5rem;
    color: #777;
    padding-right: 1rem;
  }
  .summary-single h5 {
    color: var(--main-color);
    font-size: 1.1rem;
    margin-bottom: 0rem !important;
  }
  .summary-single small {
    color: var(--text-grey);
  }
  .bday-flex {
    display: flex;
    align-items: center;
    margin-bottom: 0.3rem;
  }
  .bday-card {
    padding: 1rem;
  }
  .bday-card h4 {
    color: var(--text-grey);
    font-size: 1.5rem;
    padding-bottom: 10px;
  }
  .bday-img {
    height: 60px;
    width: 60px;
    border-radius: 50%;
    border: 3px solid #efefef;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQeik6d5EHLTi89m_CKLXyShylk4L92YflpJQ&usqp=CAU");
    margin-right: 0.8rem;
  }
  .text-center {
    text-align: center;
  }
  .text-center button {
    background: var(--main-color);
    color: #fff;
    border: 1px solid var(--main-color);
    border-radius: 4px;
    padding: 0.4rem 1rem;
    font-size: 20px;
  }
  .copyright {
    letter-spacing: 1px;
    color: black;
    font-size: 12px;
    text-align: center;
    padding-top: 25px;
  }

  @media only screen and (max-width: 1200px) {
    .sidebar {
      width: 60px;
      z-index: 150;
    }
    .sidebar .sidebar-header h3 span,
    .sidebar li span:last-child {
      display: none;
    }

    .sidebar .sidebar-header,
    .sidebar li {
      display: flex;
      justify-content: center;
    }

    .main-content {
      margin-left: 60px;
    }

    .main-content header {
      left: 60px;
      width: calc(100% - 60px);
    }
    #sidebar-toggle:checked ~ .sidebar {
      width: 240px;
    }

    #sidebar-toggle:checked ~ .sidebar .sidebar-header h3 span,
    #sidebar-toggle:checked ~ .sidebar li span:last-child {
      display: inline;
    }

    #sidebar-toggle:checked ~ .sidebar .sidebar-header {
      display: flex;
      justify-content: space-between;
    }

    #sidebar-toggle:checked ~ .sidebar li {
      display: block;
    }

    #sidebar-toggle:checked ~ .main-content {
      margin-left: 60px;
    }
    #sidebar-toggle:checked ~ .main-content header {
      left: 60px;
    }
  }
  @media only screen and (max-width: 860px) {
    .dash-cards {
      grid-template-columns: repeat(2, 1fr);
    }

    .card-single {
      margin-bottom: 1rem;
    }

    .activity-grid {
      display: block;
    }

    .summary {
      margin-top: 1.5rem;
    }
  }

  @media only screen and (max-width: 600px) {
    .dash-cards {
      grid-template-columns: 100%;
    }
  }
</style>
