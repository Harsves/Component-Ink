<script>
    import { onMount } from "svelte"
  
    let valueNr12 = 0
    let valueNr358 = 0
    let valueNr04 = 0
    let valueNr08 = 0

    onMount(() => {
    observeSection(".nr12", animateNr12)
    observeSection(".nr358", animateNr358)
    observeSection(".nr04", animateNr04)
    observeSection(".nr08", animateNr08)
  })

  function observeSection(selector, callback) {
    const target = document.querySelector(selector)
    const options = {
      threshold: 0.5,
    }

    const observer = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          callback()
        }
      })
    }, options)

    if (target) {
      observer.observe(target)
    }
  }

// Counter for .nr12
function animateNr12() {
    const intervalNr12 = setInterval(() => {
      valueNr12++

      if (valueNr12 > 12) {
        clearInterval(intervalNr12)
      }
    }, 2200 / 12)
  }
  
// Counter for .nr358
function animateNr358() {
    const intervalNr358 = setInterval(() => {
      valueNr358++

      if (valueNr358 > 358) {
        clearInterval(intervalNr358)
      }
    }, 2500 / 358)
}
  
// Counter for .nr04
function animateNr04() {
    const intervalNr04 = setInterval(() => {
      valueNr04++

      if (valueNr04 > 4) {
        clearInterval(intervalNr04)
      }
    }, 2200 / 4)
}

  
// Counter for .nr08
function animateNr08() {
    const intervalNr08 = setInterval(() => {
      valueNr08++

      if (valueNr08 > 8) {
        clearInterval(intervalNr08)
      }
    }, 2300 / 8)
}
  </script>
  
  <header>HOI</header>

<section class="numbers">
    <div class="text-area">
        <h2 class="numbers-header">We are growing and the <span class="yellow">numbers</span> speak for it</h2>
        <p>Pellentesque pellentesque dignissim vulputate tincidunt. Dis a nec pulvinar potenti elit feugiat quis
            nunc est. Sit diam laoreet pellentesque vitae vitae at dui.</p>
    </div>
<div class="numbers-flex">
<div class="numbers-wrapper">
    <div class="children-saved shapes">
        <clipPath id="childern-saved-clip">
            <svg style="--ratio: 691/1440" viewBox="0 0 691 376" fill="none"
                   xmlns="http://www.w3.org/2000/svg">
                <path
                    d="M684.891 143.32C662.595 190.92 666.685 172.221 666.608 226.409C666.556 258 667.439 289.577 667.841 321.168C667.893 325.482 667.737 329.823 667.439 334.124C667.023 340.05 663.816 343.558 657.972 344.858C638.585 349.159 619.236 353.603 599.849 357.918C575.839 363.258 551.764 368.339 527.818 373.914C520.897 375.526 514.054 376.136 507.275 374.629C486.511 370.003 465.241 369.782 444.269 367.053C398.444 361.075 352.449 356.436 306.519 351.342C276.055 347.963 245.539 344.637 215.101 341.063C193.701 338.555 172.028 338.1 150.823 333.396C141.2 331.252 131.085 331.031 121.177 330.55C100.01 329.55 79.3375 323.923 58.0672 323.949C51.99 323.962 46.1075 322.364 40.1602 321.246C32.8753 319.869 30.0055 315.84 30.0574 308.68C30.2133 289.642 30.1094 270.605 30.1094 251.554H29.8756C29.8756 235.116 29.7068 218.664 29.9406 202.226C30.0704 192.87 27.9668 184.449 23.0842 176.34C16.3837 165.242 10.4363 153.69 4.22925 142.293C2.99563 140.032 1.24259 137.693 1.03482 135.289C-0.54941 117.161 -0.00401476 98.9945 0.632276 80.8407C0.775116 76.8382 3.43714 74.6681 7.17697 73.8494C9.70914 73.3036 12.2803 72.7969 14.8514 72.6149C38.1215 70.8866 61.0928 66.6763 84.4278 65.1169C101.153 63.9863 117.775 60.4257 134.578 59.4381C157.458 58.1126 179.936 53.3306 202.869 52.239C219.217 51.4593 235.423 47.8597 251.772 46.7291C275.042 45.1048 297.936 40.3356 321.297 39.2961C337.23 38.5943 353.02 35.1897 368.953 33.9941C393.068 32.1618 416.844 27.5617 441.036 26.3402C455.255 25.6254 469.37 23.0394 483.538 21.48C516.144 17.8805 548.816 14.8137 581.371 10.7333C605.355 7.71848 629.56 6.7049 653.414 2.42958C662.309 0.844206 671.516 1.1171 680.567 0.441367C687.06 -0.039444 690.28 2.97535 690.618 9.35584C690.709 11.0842 690.929 12.8125 690.929 14.5408C690.955 50.0168 690.903 85.5058 690.981 120.995C690.994 129.052 688.215 136.225 684.891 143.32Z"
                    fill="#3DBAE1" />
                <path
                    d="M684.891 143.32C662.595 190.92 666.685 172.221 666.608 226.409C666.556 258 667.439 289.577 667.841 321.168C667.893 325.482 667.737 329.823 667.439 334.124C667.023 340.05 663.816 343.558 657.972 344.858C638.585 349.159 619.236 353.603 599.849 357.918C575.839 363.258 551.764 368.339 527.818 373.914C520.897 375.526 514.054 376.136 507.275 374.629C486.511 370.003 465.241 369.782 444.269 367.053C398.444 361.075 352.449 356.436 306.519 351.342C276.055 347.963 245.539 344.637 215.101 341.063C193.701 338.555 172.028 338.1 150.823 333.396C141.2 331.252 131.085 331.031 121.177 330.55C100.01 329.55 79.3375 323.923 58.0672 323.949C51.99 323.962 46.1075 322.364 40.1602 321.246C32.8753 319.869 30.0055 315.84 30.0574 308.68C30.2133 289.642 30.1094 270.605 30.1094 251.554H29.8756C29.8756 235.116 29.7068 218.664 29.9406 202.226C30.0704 192.87 27.9668 184.449 23.0842 176.34C16.3837 165.242 10.4363 153.69 4.22925 142.293C2.99563 140.032 1.24259 137.693 1.03482 135.289C-0.54941 117.161 -0.00401476 98.9945 0.632276 80.8407C0.775116 76.8382 3.43714 74.6681 7.17697 73.8494C9.70914 73.3036 12.2803 72.7969 14.8514 72.6149C38.1215 70.8866 61.0928 66.6763 84.4278 65.1169C101.153 63.9863 117.775 60.4257 134.578 59.4381C157.458 58.1126 179.936 53.3306 202.869 52.239C219.217 51.4593 235.423 47.8597 251.772 46.7291C275.042 45.1048 297.936 40.3356 321.297 39.2961C337.23 38.5943 353.02 35.1897 368.953 33.9941C393.068 32.1618 416.844 27.5617 441.036 26.3402C455.255 25.6254 469.37 23.0394 483.538 21.48C516.144 17.8805 548.816 14.8137 581.371 10.7333C605.355 7.71848 629.56 6.7049 653.414 2.42958C662.309 0.844206 671.516 1.1171 680.567 0.441367C687.06 -0.039444 690.28 2.97535 690.618 9.35584C690.709 11.0842 690.929 12.8125 690.929 14.5408C690.955 50.0168 690.903 85.5058 690.981 120.995C690.994 129.052 688.215 136.225 684.891 143.32Z"
                    class="filled" />
            </svg>
            <div class="stats-numbers nr358">{valueNr358}</div>
            <p>Children saved</p>
        </clipPath>
    </div>
        

        <div class="talents-discovered shapes">
            <clipPath id="talents-discovered-clip">
                <svg style="--ratio: 254/1440" viewBox="0 0 254 332" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M253.872 25.5571C253.859 67.9724 253.872 110.401 253.872 152.829H253.846C253.846 198.285 253.885 243.741 253.82 289.184C253.794 304.31 253.626 304.765 238.614 308.235C212.526 314.264 186.335 319.813 160.195 325.622C151.767 327.493 143.431 329.832 134.938 331.353C126.212 332.912 124.082 331.314 123.407 322.282C122.758 313.667 123.082 304.973 122.965 296.318C122.913 292.433 123.069 288.508 122.641 284.649C121.732 276.241 119.589 274.097 111.382 273.317C107.526 272.954 103.604 273.084 99.7083 273.071C72.4517 273.058 45.195 273.175 17.9384 273.019C3.19987 272.941 2.00524 270.952 0.849529 256.593C-1.16323 231.747 2.86225 208.512 15.9127 186.94C24.1715 173.296 26.8985 158.43 26.5089 142.277C25.6908 107.672 26.2102 73.0274 26.3011 38.396C26.3531 23.5559 28.6386 21.7236 43.481 20.1642C76.9836 16.6556 110.447 12.7181 143.924 8.93661C147.794 8.50778 151.65 7.71509 155.52 7.6761C182.413 7.44219 208.864 2.45219 235.602 0.554934C238.186 0.373006 240.783 -0.0688378 243.354 0.00913152C251.249 0.230044 253.301 2.06234 253.833 9.97622C254.184 15.1482 253.872 20.3591 253.872 25.5571Z"
                        fill="#FFDA1D" />
                    <path
                        d="M253.872 25.5571C253.859 67.9724 253.872 110.401 253.872 152.829H253.846C253.846 198.285 253.885 243.741 253.82 289.184C253.794 304.31 253.626 304.765 238.614 308.235C212.526 314.264 186.335 319.813 160.195 325.622C151.767 327.493 143.431 329.832 134.938 331.353C126.212 332.912 124.082 331.314 123.407 322.282C122.758 313.667 123.082 304.973 122.965 296.318C122.913 292.433 123.069 288.508 122.641 284.649C121.732 276.241 119.589 274.097 111.382 273.317C107.526 272.954 103.604 273.084 99.7083 273.071C72.4517 273.058 45.195 273.175 17.9384 273.019C3.19987 272.941 2.00524 270.952 0.849529 256.593C-1.16323 231.747 2.86225 208.512 15.9127 186.94C24.1715 173.296 26.8985 158.43 26.5089 142.277C25.6908 107.672 26.2102 73.0274 26.3011 38.396C26.3531 23.5559 28.6386 21.7236 43.481 20.1642C76.9836 16.6556 110.447 12.7181 143.924 8.93661C147.794 8.50778 151.65 7.71509 155.52 7.6761C182.413 7.44219 208.864 2.45219 235.602 0.554934C238.186 0.373006 240.783 -0.0688378 243.354 0.00913152C251.249 0.230044 253.301 2.06234 253.833 9.97622C254.184 15.1482 253.872 20.3591 253.872 25.5571Z"
                        class="filled" />
                </svg>
                <div class="stats-numbers nr12">{valueNr12}</div>
                <p>Talents discovered</p>
            </clipPath>
        </div>

        <div class="new-partners shapes">
            <clipPath id="new-partners-clip">
                <svg style="--ratio: 445/1440" viewBox="0 0 445 282" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M444.252 60.5536C443.473 75.2118 443.188 90.078 440.409 104.424C436.279 125.762 436.877 147.489 433.241 168.788C429.241 192.218 430.046 216.18 424.995 239.532C423.19 247.888 424.099 256.802 423.086 265.366C421.385 279.673 419.45 281.532 405.166 281.778C386.142 282.103 367.118 281.857 348.082 281.857V281.921C329.058 281.921 310.021 282.142 290.997 281.844C277.207 281.636 276.311 280.336 276.518 266.86C276.778 249.551 277.298 232.255 280.583 215.18C281.076 212.646 281.362 210.034 281.492 207.448C282.167 194.791 279.271 191.36 266.325 190.087C257.741 189.229 249.08 188.449 240.51 188.033C218.902 186.981 197.813 181.965 176.153 181.172C158.922 180.548 141.781 177.637 124.601 175.792C89.8647 172.076 55.1155 168.398 20.3792 164.695C17.3666 164.383 14.3669 163.98 11.3542 163.707C4.57581 163.083 1.4593 158.912 0.900924 152.596C0.537329 148.295 0.342547 143.942 0.576286 139.641C2.77084 99.8632 2.62798 60.0598 2.77082 20.2565C2.84873 -0.45738 3.73176 -1.30198 24.145 1.07608C65.7376 5.92317 107.291 11.1471 148.884 15.9422C178.893 19.3989 209.033 21.7509 238.938 25.8573C259.469 28.6642 280.18 29.3139 300.646 33.2904C314.917 36.0583 329.876 35.2916 344.42 37.7476C367.404 41.6201 390.882 41.5291 413.775 46.4931C420.021 47.8576 426.722 47.0649 433.137 47.8186C441.902 48.8582 444.707 51.7431 444.252 60.5536Z"
                        fill="white" />
                    <path
                        d="M444.252 60.5536C443.473 75.2118 443.188 90.078 440.409 104.424C436.279 125.762 436.877 147.489 433.241 168.788C429.241 192.218 430.046 216.18 424.995 239.532C423.19 247.888 424.099 256.802 423.086 265.366C421.385 279.673 419.45 281.532 405.166 281.778C386.142 282.103 367.118 281.857 348.082 281.857V281.921C329.058 281.921 310.021 282.142 290.997 281.844C277.207 281.636 276.311 280.336 276.518 266.86C276.778 249.551 277.298 232.255 280.583 215.18C281.076 212.646 281.362 210.034 281.492 207.448C282.167 194.791 279.271 191.36 266.325 190.087C257.741 189.229 249.08 188.449 240.51 188.033C218.902 186.981 197.813 181.965 176.153 181.172C158.922 180.548 141.781 177.637 124.601 175.792C89.8647 172.076 55.1155 168.398 20.3792 164.695C17.3666 164.383 14.3669 163.98 11.3542 163.707C4.57581 163.083 1.4593 158.912 0.900924 152.596C0.537329 148.295 0.342547 143.942 0.576286 139.641C2.77084 99.8632 2.62798 60.0598 2.77082 20.2565C2.84873 -0.45738 3.73176 -1.30198 24.145 1.07608C65.7376 5.92317 107.291 11.1471 148.884 15.9422C178.893 19.3989 209.033 21.7509 238.938 25.8573C259.469 28.6642 280.18 29.3139 300.646 33.2904C314.917 36.0583 329.876 35.2916 344.42 37.7476C367.404 41.6201 390.882 41.5291 413.775 46.4931C420.021 47.8576 426.722 47.0649 433.137 47.8186C441.902 48.8582 444.707 51.7431 444.252 60.5536Z"
                        class="filled" />
                </svg>
                <div class="stats-numbers nr04">{valueNr04}</div>
                <p>New partners</p>
            </clipPath>
        </div>

        <div class="clubs-invested shapes">
            <clipPath id="clubs-invested-clip">
                <svg style="--ratio: 470/1440" viewBox="0 0 470 348" fill="none"
                    xmlns="http://www.w3.org/2000/svg">
                    <path
                        d="M469.69 138.387C469.677 166.079 469.69 193.758 469.664 221.437C469.664 225.336 469.573 229.234 469.352 233.107C469.04 238.396 466.794 241.683 461.041 242.944C443.745 246.751 426.591 251.143 409.359 255.172C375.298 263.138 341.224 271.013 307.163 278.927C274.349 286.542 241.534 294.17 208.707 301.759C173.789 309.841 138.858 317.872 103.927 325.916C74.904 332.608 45.8943 339.379 16.8457 345.954C1.71762 349.372 -0.386035 347.436 1.18521 332.413C2.08121 323.811 3.13307 315.221 4.05504 306.632C8.74281 263.229 13.4955 219.826 18.0145 176.397C19.1312 165.65 19.2091 154.799 20.2869 144.053C21.4946 132.006 23.3255 131.24 35.1424 128.901C58.8799 124.222 82.4486 118.765 106.082 113.58C138.13 106.536 170.218 99.6751 202.175 92.2551C216.446 88.9544 217.394 87.304 217.537 72.8407C217.719 54.245 217.381 35.6364 217.563 17.0407C217.706 2.39546 219.485 0.537237 234.054 0.277339C249.611 -0.0215433 265.181 -0.0215686 280.737 0.251324C295.775 0.524216 297.398 2.34346 297.645 18.0023C297.839 30.5424 297.476 43.0954 297.813 55.6225C298.177 69.1112 300.696 70.6836 313.578 67.7467C358.625 57.4808 403.697 47.3447 448.77 37.1697C449.186 37.0658 449.614 36.9749 450.03 36.8969C468.092 33.5832 469.638 34.7788 469.677 52.7507C469.729 81.3004 469.69 109.837 469.69 138.387Z"
                        fill="#163A3A" />
                    <path
                        d="M469.69 138.387C469.677 166.079 469.69 193.758 469.664 221.437C469.664 225.336 469.573 229.234 469.352 233.107C469.04 238.396 466.794 241.683 461.041 242.944C443.745 246.751 426.591 251.143 409.359 255.172C375.298 263.138 341.224 271.013 307.163 278.927C274.349 286.542 241.534 294.17 208.707 301.759C173.789 309.841 138.858 317.872 103.927 325.916C74.904 332.608 45.8943 339.379 16.8457 345.954C1.71762 349.372 -0.386035 347.436 1.18521 332.413C2.08121 323.811 3.13307 315.221 4.05504 306.632C8.74281 263.229 13.4955 219.826 18.0145 176.397C19.1312 165.65 19.2091 154.799 20.2869 144.053C21.4946 132.006 23.3255 131.24 35.1424 128.901C58.8799 124.222 82.4486 118.765 106.082 113.58C138.13 106.536 170.218 99.6751 202.175 92.2551C216.446 88.9544 217.394 87.304 217.537 72.8407C217.719 54.245 217.381 35.6364 217.563 17.0407C217.706 2.39546 219.485 0.537237 234.054 0.277339C249.611 -0.0215433 265.181 -0.0215686 280.737 0.251324C295.775 0.524216 297.398 2.34346 297.645 18.0023C297.839 30.5424 297.476 43.0954 297.813 55.6225C298.177 69.1112 300.696 70.6836 313.578 67.7467C358.625 57.4808 403.697 47.3447 448.77 37.1697C449.186 37.0658 449.614 36.9749 450.03 36.8969C468.092 33.5832 469.638 34.7788 469.677 52.7507C469.729 81.3004 469.69 109.837 469.69 138.387Z"
                        class="filled" />
                </svg>
                <div class="stats-numbers nr08">{valueNr08}</div>
                <p>Clubs invested</p>
            </clipPath>
        </div>
     
    </div>
</div>
</section>

<style>

    header {
        height: 100vh;
    }

* {
    box-sizing: border-box;
    list-style: none;
    margin: 0;
    padding: 0;
}

.numbers {
    padding: 2em;
    color: white;
    background-color: #051A1A;
    font-family: 'Kirang Haerang';
    overflow: hidden;
    height: 100vh;
}

.numbers-flex {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    position: relative;
    top: 15%
}

.numbers p {
    font-family: "Apercu pro";
}

.numbers-wrapper {
    max-height: 100%;
    max-width: 100%;
    display: grid;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    padding: 10%;
    grid-template-areas:
    "partners children"
    "clubs talents";
}

.numbers-wrapper p {
    font-size: clamp(13px, 1.1vw, 85px);
}

.shapes {
    width: max-content;
    height: max-content;
}

@-webkit-keyframes fillAnimation {
  0% {
    stroke-dashoffset: 500%;
    opacity: 0;
  }

  100% {
    stroke-dashoffset: 0;
    opacity: 1;
  }
}

@keyframes fillAnimation {
  0% {
    stroke-dashoffset: 500%;
    opacity: 0;
  }

  100% {
    stroke-dashoffset: 0;
    opacity: 1;
  }
}

.children-saved {
    color: white;
    position: relative;
    clip-path: url(#children-saved-clip);
    grid-area: children;
    transform: translateX(-124%) translateY(-18%);
    width: 50%;
}

.children-saved path {
    fill: #3DBAE1;
    stroke: currentColor;
    stroke-width: 5px;
    animation: fillAnimation 4s ease-in-out;
    stroke-dasharray: 500%; 
    stroke-dashoffset: 150%;
}

.children-saved p {
    position: absolute;
    bottom: -27%;
    right: -12%;
}

.nr358 {
    position: absolute;
    bottom: 100%;
    right: -3%;
    color: var(--justWhite);
    content: "{valueNr358}";
    transition: content 5s;
}

.talents-discovered {
    position: relative;
    grid-area: talents;
    clip-path: url(#talents-discovered-clip);
    transform: translateX(-66%) translateY(10%);
}

.talents-discovered path {
    fill: #FFDA1D;
    stroke: currentColor;
    stroke-width: 5px;
    animation: fillAnimation 4s ease-in-out;
    stroke-dasharray: 510%; 
    stroke-dashoffset: 140%;
}

.talents-discovered p {
    position: absolute;
    bottom: 31%;
    right: 84%;
    color: black;
    max-width: 20%;
}

.nr12 {
    position: absolute;
    top: 55%;
    right: 2%;
    color: black;
    content: "{valueNr12}"; /* Initial value */
    transition: content 5s;
}

.new-partners {
    position: relative;
    grid-area: partners;
    clip-path: url(#new-partners-clip);
    transform: translateX(-28%) translateY(-38%);
    color: black;
}

.new-partners path {
    fill: #d3d3d3;
    stroke: white;
    stroke-width: 5px;
    animation: fillAnimation 4s ease-in-out;
    stroke-dasharray: 510%; 
    stroke-dashoffset: 140%;
}

.new-partners p {
    position: absolute;
    bottom: -8%;
    right: 35%;
    color: var(--charcoal);
    transform: rotate(5deg);
}

.nr04 {
    position: absolute;
    top: -15%;
    right: 25%;
    transform: rotate(6deg);
    color: var(--justWhite);
    content: "{valueNr04}"; /* Initial value */
    transition: content 5s;
}

.clubs-invested {
    position: relative;
    grid-area: clubs;
    clip-path: url(#clubs-invested-clip);
    transform: translateX(-23%) translateY(-22%);
}

.clubs-invested path {
    fill: #163A3A;
    stroke: currentColor;
    stroke-width: 5px;
    animation: fillAnimation 4s ease-in-out;
    stroke-dasharray: 510%; 
    stroke-dashoffset: 140%;
}

.clubs-invested p {
    position: absolute;
    bottom: 80%;
    left: 2%;
    transform: rotate(5deg) translateX(40%) translateY(-180%);
}

.nr08 {
    position: absolute;
    top: 70%;
    right: 30%;
    transform: rotate(-10deg);
    color: white;
    content: "{valueNr08}"; /* Initial value */
    transition: content 5s;
}


.children-saved svg,
.talents-discovered svg,
.new-partners svg,
.clubs-invested svg {
    transform: rotate(90deg);
    width: calc(var(--ratio) * 175vw);
    height: auto;
    overflow: visible;
}

.stats-numbers {
    position: absolute;
    font-size: 10vw;
}

@media only screen and (min-width: 560px) {
    .children-saved svg,
    .talents-discovered svg,
    .new-partners svg,
    .clubs-invested svg {
        transform: rotate(0deg);
        width: calc(var(--ratio) * 85vw);
    }

    .numbers-wrapper {
        grid-template-areas:
        "children talents"
        "partners clubs";
    }

    .children-saved {
        transform: translateX(-25%) translateY(-18%);
    }

    .children-saved p {    
        bottom: 9%;
        right: -87%;
        transform: rotate(-13deg);
    }

    .nr358 {
        bottom: 35%;
        right: 4%;
        transform: rotate(-6deg);
    }

    .talents-discovered {
        transform: translateX(-35%) translateY(-28%);
    }

    .talents-discovered p {
        bottom: 9%;
        right: 25%;
        transform: rotate(-12deg);
    }

    .nr12 {
        top: -5%;
        right: 5%;
    }

    .new-partners {
        transform: translateX(-13%) translateY(-38%);
    }

    .new-partners p {
        bottom: 7%;
        right: 8%;
        transform: rotate(0deg);
    }

    .nr04 {
        top: 5%;
        right: 5%;
        transform: rotate(6deg);
    }

    .clubs-invested {
        transform: translateX(-63%) translateY(-50%);
    }

    .clubs-invested p {
        bottom: 11%;
        left: 5%;
        transform: rotate(-12deg);
    }

    .nr08 {
        top: 7%;
        right: 5%;
        transform: rotate(-14deg);
    }
}

</style>