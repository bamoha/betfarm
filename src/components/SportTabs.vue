<template>
  <div>
    <ul class="nav nav-pills mb-3 justify-content-around" id="pills-tab" role="tablist">
      <li class="nav-item">
        <a
          class="nav-link active"
          id="pills-home-tab"
          data-toggle="pill"
          href="#pills-home"
          role="tab"
          aria-controls="pills-home"
          aria-selected="true"
          @click="getPickedSport('Football')"
        >
          <div class="sport-circle"></div>
          <span class="sport-name">Football</span>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          id="pills-home-tab"
          data-toggle="pill"
          href="#pills-home"
          role="tab"
          aria-controls="pills-home"
          aria-selected="true"
          @click="getPickedSport('Tennis')"
        >
          <div class="sport-circle"></div>
          <span class="sport-name">Tennis</span>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          id="pills-home-tab"
          data-toggle="pill"
          href="#pills-home"
          role="tab"
          aria-controls="pills-home"
          aria-selected="true"
          @click="getPickedSport('BasketBall')"
        >
          <div class="sport-circle"></div>
          <span class="sport-name">BasketBall</span>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          id="pills-home-tab"
          data-toggle="pill"
          href="#pills-home"
          role="tab"
          aria-controls="pills-home"
          aria-selected="true"
          @click="getPickedSport('Volley')"
        >
          <div class="sport-circle"></div>
          <span class="sport-name">Volley</span>
        </a>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent">
      <div
        class="tab-pane fade show px-3 py-2 active"
        id="pills-home"
        role="tabpanel"
        aria-labelledby="pills-home-tab"
      >
        <span class="picked-tab">{{pickedSport}}</span>
      </div>
    </div>
    <div>
      <b-tabs content-class="mt-3" class="data-tabs">
        <b-tab title="Match Result" active>
          <div class="competition-name">
            <div class="competition-logo"></div>
            <span>European championship</span>
            <span>1</span>
            <span>x</span>
            <span>2</span>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
        </b-tab>
        <b-tab title="Double Chance">
          <div class="competition-name">
            <div class="competition-logo"></div>
            <span>European championship</span>
            <span>1</span>
            <span>x</span>
            <span>2</span>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
        </b-tab>
        <b-tab title="Draw No Bet">
          <div class="competition-name">
            <div class="competition-logo"></div>
            <span>European championship</span>
            <span>1</span>
            <span>x</span>
            <span>2</span>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
          <div class="row match">
            <div class="col-5">
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>Gerogia</span>
                <span>0</span>
              </div>
              <div class="d-flex justify-content-between align-items-center my-2">
                <span>1st Half 35”</span>
                <span>
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.9584 6.13752C15.8536 5.81354 15.5663 5.58343 15.2263 5.55279L10.6082 5.13347L8.78215 0.859312C8.6475 0.546072 8.34085 0.343307 8.00014 0.343307C7.65944 0.343307 7.35279 0.546071 7.21814 0.860044L5.39204 5.13347L0.773272 5.55279C0.433908 5.58416 0.14728 5.81354 0.0419302 6.13752C-0.0634192 6.46151 0.0338734 6.81686 0.290594 7.04087L3.78128 10.1022L2.75196 14.6364C2.67664 14.9698 2.80604 15.3144 3.08266 15.5144C3.23134 15.6218 3.4053 15.6765 3.58072 15.6765C3.73197 15.6765 3.88199 15.6357 4.01664 15.5551L8.00014 13.1743L11.9822 15.5551C12.2736 15.7304 12.6409 15.7144 12.9169 15.5144C13.1936 15.3138 13.3229 14.969 13.2476 14.6364L12.2183 10.1022L15.709 7.04148C15.9657 6.81686 16.0637 6.46212 15.9584 6.13752Z"
                      fill="#272727"
                    />
                  </svg>
                </span>
              </div>
            </div>
            <div class="col-7 d-flex justify-content-center align-items-center">
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>2.16</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
                <div class="event-price d-flex justify-content-center align-items-center">
                    <span>3.26</span>
                </div>
            </div>
          </div>
        </b-tab>
      </b-tabs>
    </div>
    <div class="d-flex justify-content-between px-3 bet-buttons">
        <b-button class="nav-btn login">Book Bet</b-button>
        <b-button class="nav-btn login">Bet Slip (0)</b-button>
    </div>
  </div>
</template>

<script>
export default {
  name: "SportTabs",
  data() {
    return {
      pickedSport: "Football"
    };
  },
  methods: {
    getPickedSport: function(sport) {
      this.pickedSport = sport;
    }
  }
};
</script>