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
    background-image: url("https://scontent.fcmb4-2.fna.fbcdn.net/v/t39.30808-6/250092557_1796773993852287_7146782582643226627_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=iCUlBqJG-T4AX_Aefra&_nc_ht=scontent.fcmb4-2.fna&oh=00_AT8hkLGOsGWOSdKfCOaLvMrPSp7VA0H4J5AxqyNcyWO0VA&oe=62A2B428");
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
    background-image: url("data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAoHCBUSEhUREhUSEhIRERESEhERERERERERGBQZGRgUGBgcIS4lHB4rHxgYJjgmKy8xNTU1GiQ7QDszPy40NTEBDAwMEA8QHhISHDQhJCQ0NDQ0NDE0NDQ0NDExNDE0NDQ0MTQ0MTQ0MTQ0NDE0NDQ0NDQ0MTQ0NDQ0NDQxNDQ0NP/AABEIARMAtwMBIgACEQEDEQH/xAAcAAABBQEBAQAAAAAAAAAAAAADAAIEBQYBBwj/xAA8EAACAQIDBgMFBQcEAwAAAAABAgADEQQSIQUGMUFRYSJxkRMygaGxI0JScsEHFTNi0eHwFCRDsoKSov/EABoBAAMBAQEBAAAAAAAAAAAAAAABAgMEBQb/xAAnEQACAgIBAwQDAAMAAAAAAAAAAQIRAyESBDFBEzJRcSJhoTOBkf/aAAwDAQACEQMRAD8AyyYc9YanhT1iSSEjsniFp4Y9Y8YUzqGHUw5C4kdsGbSHiMCZb6xeyvHY1Eo6WzWvJdHZzS6oYaTEw0XIOBRJs1ryww2BZTcSyWjDosdicDlKowEZXdzJOSc9mYWHAzmMw7GVbYRrzYVqEhthdYWCiVFHDtbhGPhW6TQJQtE9GFhxZnhhm6QdbCk8poTSgKiQsXFmYfAnpAPgzbhNG4kdxCx8WZephyOUHkNuEv6lO8F/pomxqJmaqnpFL6rgu05FY+I+m4k2kJmaONk+lj4FGiprJCLM+u0e8Ou0+8Qy+VIVElGm1B1hE2oOsANHRWS0WZqltYdZLTaw6wAvQkIqSjXaw6wTbwhD4iMsAo0qpHZJnKW8gbgNOp0kuntxGgFMsnpwDJIdXbKDiyjzNoEbXQ8CD5XPzgFFnljGEh/vEdYxtojrAZKZYGokjttEQTbREAO1UkWok7Ux4kZ8aIAdKRyJIxxgiGNEBEl0ikZsaIoAYBbwyM00ezdgCpbQmXlPcsnlJbBGDLv1jDXcc5u8Rufl5GZvauxjSPaCYyoGKfrHjFv1hqOEzScmxrjjrDkg4srlxr9YZce/WS12I9+GkPU2WKQzN2/tBSTDiztGo1gWY6jrIL1C7acSeJ5CSX5kEFSpAt+UysVGubdLfQywCtiiugueV+sam02B++PJv0nBQaxAGui+oH9DI1bDFRz/AM5ntACYmLDdbniTYk/GScDtBzUyA+H6SkTv8gfreWWDAuLA37m0ALKvtF16yP8AvZ5JxlPMoYlQTpYWv2lZ7AyXoO5K/ejd5w7SbvBJhCYVdnOdALwsKGNtFu8G20GlrR3ZrONF9Yq26mIUXKj5xWBUHaBjf3iY7E7PembMtpENKOxUHO0TFIxpxQsKPcN2dmhaam2pAmop4UAcJB2Cn2aflH0l4qxRVqwkypxmEBHCeeb2YYANp1nqOJEwu+FC1Jm8/oZm3TKirRgtl0QbS4SkLgSgwtQpYiTBjzmEpoqMjV0qKheF+g5k9JQ7xMEZUJAIGY24gnQWkzB4/TMxtlF5mMfihXru+pHfko0AihGnY5O1RJw2FNdlVAx68zNLh9yibG+XzEu9y9kqlIVCBmbX4cpp3tG5MFFGLO6KLcg9Jn9qbruLhfFPSnEjVFk8maqMTxzE7t1l1ynyErRh2VrEsjdwR857gaIPECZ7eHd5aiF6YAYC+nOCm/IpYl4MNgK5By1LZrWDEA38jJAoi/EafOQqbrnNN9NbA8gZZ4WjdgDc25X4jtNJPRlFbLPZezC9rDTraaTZ+wbOCRJ+79BPZqR2B/rNPSw4nP6jbNnjSWyJhcAAOA9ITEYAMLWliqWhCJ0J2jmkqZ55t3dzODYfKYuruy4J/pPbMRRB5StqbPB5TOVp6Li15PG6m7riKer1dmr0ik8pFfiWOwh9mv5RLtBKjYi/Zr5CXSCbx7GEu5GxAmJ33NqB+P0M3tRJjd+aF6Ddgx/+TM5LZUXo8hR45KnikZ1InaQOaasSLrDNcEdRaVOFpH2pXkDnqHteyLLDDkjzPyHWSNh4cVa9KmP+SoXqHmVWTdI0Suj1Td9CMOgI1yiSnGsHXdEp5S/s1A1ynKxFuAPL4TG496JYtQr1ab8mFd3F+6sSDMm0u5sot9jYuRAsJQ7FxWIZslUrUHKootcdxyMs9o1XpoSoueQkci+IdliyXB8pkPbYmo32mIWipPuU0UtbuzTQ7KR1X+M1dfvK4TOO6lQPQwTT8jaa8HlG9dELXdl0sx4ecbs7E1LZlIbLa6nj5jrLb9oFAJicw92oobhpfUa+kotkVMrW9B2/D/Sbx3E53qR6Bu9t4KFFS6dDxXjfiNPWegYLHo6gqwIPCxvPJqRtYrwP+WPIybg9pvRbw+7zT7vmBymEsbu4mqyKqketJXBnfaiYWhvQo0a485NXeFDwYesIuS7omUYvaZrWqCBdxKvD4vOAeskuwtLUmzJqgjuIpW13twiitjos9hn7NfIS7SZXdvGBqaWPITSU6om0JaMpLYd5k98xeg/5G/6maSrWAExG+G0hkZAeII9dJMnbocUeYVKNzO0cNrLBEvH5LGWwRXbSBp0yw+8MvlLf9naXxlz/AMdE/AkgSr24bqifif8ASW37PAf9U7/dIanfv7w+kiWkaw2z0Lbex0xSZKgZlGtldk9cp1mNxm5tNTemKyEfhcn5k3no6cNZExLqouZn9OjVb01ZS7rbMel77M3IZwoI9JY7YplkYLo2tjLHZbiomcCy3IUn71ja/reMrUyysQMxF9BxPaFXEOT5HmT7v1KjEvVqISeKUwAR00N/nLXYm7dSjUVxiHKD3kKKA3xH11mlwtRKgDLwPIixB5gjkZLVAIttd9FaT7bPO/2m0f4bdmHzE8+w1SzeX0no/wC0WoCEQ8Tn/T+k8xDansSPheaY3owyqpWbjZNYOhHUX8mHH9IarWGnlKHYeJs69G0+PKWePXw3HDWWkS3oLUxSmQ3qAEWPPrKwVjONWN46Is9m2Tb2aW/Cv0lwEBE893d28DTVSdVAE0j7bCre44TNLwU/klYlIpl8RvCW5iKacTPmQdg7aNAZT7v0moTe1AOMwMcrw9NMfJm0xm9ZYWUWmZxddqhuxgFa8IqSowSJcmJEhDThESSEpyuJPJmZ3h8OTzf6CT9w9qpTqrRcENVdSjDhmykFTIu9qWVDzDn0t/eZrD12Qq6e/Tdai+am4+YmU1ejoxyrZ9BVK1heZzF4w1ahQMFRf4jsQqgdLmWGFxa16KVU1WogYfEcPhwmP2rs1lc4rJ7WmtSz0mY5bA8e2l9eoE5HbdHdjSNomJp5UFOuoye6EqJlbsQdDEmKa4+0ysL+HNT1v15yswL7NrouemtAiylaqLTIupNy406a36QGKwWyqShy6NbJ7jPUJzPawC37+spxY08f7/4EZmoVTe+Wob35ZiZc06+YTAYOn7atfDGsmFR1v7QnK7crKfd1+OnebSl4R5TN2nQ2kYz9omIVCDcZsllF9bljraeb0eNvOaDfLaAr4yoQbqi+yU30uupP/sSPhKBBr6GdeONRODLLlItMKCLEdfQ8po2fPTBHTXsZnMMwPk2h7HkZe7Je5KNodfXnKXcT7EJ8L/nKBbDTTPge0A+B7TWjBszqBkN1JB7QlbG1WFixtLR8HItTCQ4i5FWcQ4PGckmth4oUFlqHvC01nKNGTqOHiKOU0kqnThaVCTKdGOxUBSlDrTklKUL7KFhRk9r0faZy3uqoA9df09JiqRsb8Rwbym33kf2dNwOerdteExBOSogI94eIfmPCZvZstG7/AGd7WyFsHUN11qUT2PvJ+vrPRqOEQo6MLo5N/jPHty6ZONRRrZapF+gW1u09V2ZtIAmlU8Lcs2h/v5iYSSUjog3WikxeExNAlERK1K5yqVpuvHjlbVT2BtISYTE12yGimHQnxMtOnTI4cGN2HD7s3FVVMCKQEh38nWuotbir+aItDZyUkSnTFlQ3J5s3MmZffXbow1M00P2tQEJb7o5uf07zSbR2hl8FPVubch/eeWb9ofaIxJJYNcmEEpSownJqLl5MmEJ78z1iR9YV18Ib8WkigWNj1nWcJY0KgBseekt8ExqMqqctTUKeHjXUeouPjM+w+f1El7NqkVBfkfnwiopM3mx9pCp4KgyVFOUg6XbpbkZbvhx0mSqKTasDmKr4r+8yDvzIGoPbymw2ZV9pTDHiND5iXGREo+SBVw0hVcNL6rTkKtTjszoz1fDRSxrU52FhQKgksKKSLQEsaIhQ7DU6clIkZTWSkWADkSEancEXtccRyjlWPZgouxAA5nSIa26Rj95tl1WCKqFqakscguS3InrM+2FpmmyuCKgIYXXxAj7p6TZ7W3lRAVp2Lfibh8BzmFxeNZ3LXvmOrfDlIk6O+HSZGlKSpf0tNzCtLGozkfaBkBPItw+Yno2MwgY6gHzAM8hR73buMtuVuFps9ib6Cy08VcFbBaoFwR/OOveYTi3s7JdK4RUo7LzE+0p+4xAHI6iRkxNVuLXHQC0tRi0qrmVldT95SCJHZlHCc8tGS/aI+SwJmD34F8rdDabvGYpKaFnZVsOZnmO8e0Pb1PD7i6L37zTDF3ZOSNqigAvpfT6GLLqB0iW17EX+UNUQDS3Hvedh57VE/bGANIr0dFqL6WYeo+cirZAjcc63bscxFvlLbE7XTEYZEYZa1AgK3J0tYi/obdpUNTvboDfyMANFgK5FMk6gpU/6kfrNRu/dqIdTrzHJhMtsmomRqdQ5cysgY8Fvwl3svG/6e1OoCgbRX+4/k3C/aJFM0lwyg9ZErLC0n963C4YfEf2g60oxZXVhOR1adjAZQEsaAkCgJY0RHYiXSE7jMalCn7Spe1wLAXJJ6CCr4laSF25cB1PSYvbO0mq3udOQ5Adomzu6To5Zrk9Jf0vMRvmAD7Omb8i5FvQTPbR27WrHxNYfhXQSqYmMBibPVx4IYuy2Gzk8Tfz1itoRyJv5RiwqiQdSipKmJTYWgnMMYxxBouS1Q2jiXpm9NmQ/ysRJDbZxBFjVe3mJEKThWQ4pnNKF90crV3f32ZvMkyO4hysGyx0ZShoiVKfMQbqx58PWS2WDNOUmcGXp+W0RLm4/zSSqdT1+sG9KCsRHZyShKLplthqov4hp16TR4EComRScraNTPiQ8jYHgfKY2nWI4y/3exwpuL3Kkg68u8YKLejTbvV2Gei5uabGmGPMDUfGxlrWlLsKoKhqvzNeo3ca2HyEuXbSNGUlsg1p2NrmdjIFQljRlXRaTRWCqzHgqk+ggUlbood49oZqnswfDT0825zPVHvOYjEFmZjxZifUwBeZtn0mNrHjUF4HXnQI1YRRAqOxywimDEeDA3i6HmMM7eNMCmxtpwrHRRENIGViyx8UCeKBMkYUhyI0iBEoIAUg2oyVaNIgYywxktkI0YZCdB0j2MSmOzD0IWajdzBpWVhmdKi+IOjFSR36y3wzujmjUOZrZke1s68DcdRp6zNbuYr2ddDyY5D5H+9pqttCwWoONNw3/AIHwsPQ/KUjh6vEoSVdmgVcTs5WaclHER6LTm2K2XDv3AX1M5RMjbxP9h5usGa4VeRfZk2M4JwmIGZs9nlsOIYCRA2o7iTFGkR1YXys4J0GNivA0sfecM5FAqzsUUUAORRGcJgSKciM5eBLZ2NaOWMqcCegiFL22BbjGgxE8Y28Zxt7JNCoVII4ggjzE9Arn2lL86D5iedK03mzql6FM/wAglROXrdwT+GcqcBfjFG1mnZZ5ZHpNIW8jfYj84+kPSaQN4n+zQdW/SD7G2D/IjPXnCYoxjMz03KkOpN4u/ASz4CU9I+MectS0TOjo5XF/YjOXiMbeNHU5DgZ28ZedBgCkOvO3jLxXiHyHExpMRM4TATkdvOXnLxpMZm5BAZx+HwMaDFiDZSe0kHL8W/ghK8cDAIYUGUebGdoIpm12W/8At0/LMQpmx2W/+3TyMaM+qdwX2HqtFBVWilnnAKZlfvAfAnmfpJqNIO3taano36QfY1wupoorxrmdJg2MzO6UtD8L74liWlZhj4h8ZPLQZ09JKoP7HExXg80WaB0cwl4rwYadvAakEvFeMzRZoh8h95yNvOExg5HWM5eNvOXiM3IIJzFnwHzH1iBg8Y3gt1IgKcqxv6ZCWFBgVhAYzzIsIpms2cbUE8rzJJrp10mxRMqKvRQPlKiLqJfikDqvOwdWKUcQxGkTbb/ZgfzQytIe2D4F84M0xe5FOTGMZ0wbGZnVJnVaxB6GTS0gSzxNOyow0zoCR3EC8M6tAs05mg805eBt6gXNOh4G8V4hrIHzTueAzRZoFeqHzxpaCzRZoCeULmizQWaLNAXqBlaBxj8B01j1kSq12J7xonPkqFfIlhBAqYVYHLFk7ZdHPVUcgcx8hNU5lNu/SsGqdfCJZu8pGWaVuvga8UGzRSjEjrIm1j4B5w6NIu1NUB6GJl4/cioJjCZ1oyQayY6mtyBxuQJoNs2ApIBbLT1+Mg7GwhaorHQA3lhvC/jUDkusfgvE6mimZYMiFBiI7RHRKKe0CivH2igTQy8V46KAq/Y2KOnbQHxY0CPVJwCOBgXGK8hVsOPCV7yZUPhMgkwRl1L2kOWEWCElYOnmdR1PygYxZpNnpkpKDxIufjCs0aW5QbNLOeTt2JmigmaKAgSmSqFNXurAEW4GQlaS8K1ryZdioe5A6+z6S8FlZiVVfdAEs8S8pMW+szjbOiTLPY9YAktwVbyFi6/tKjP1OnlA0KtkYfi0+EaTNGXiVLkK8V428V4jRyOkzk5eK8CbHaRXjbxQHyO3nY2K8AsdeKcE7eA0zma4I56yLDn3oVaYbjC6MJ3L/RFWWux6fiL8gLfGBXZxPukfGW9CkKahRy49zGtmcnxQYtBs0TNBs0oxGu0UGxigA2nJeH5xRSZdioe5AcTKbE8YopETaXY5T4Toiils2j7UcM5FFESxTgiigB2ciigMUUUUAOzoiigCGc/SSMLFFB9iC3wsM0UUcexhk7gmg2iilEA2iiigB//Z");
  }
  .img-3 {
    background-image: url("data:image/jpeg;base64,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");
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
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYZxEcLn9GPG9z7cMn4DqQ1W1HwIQa6rG8ug&usqp=CAU");
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
