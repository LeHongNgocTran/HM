<script>
import HeaderPublic from "../../components/PublicHeader.vue";
import PublicFooters from "../../components/PublicFooters.vue";
export default {
  components: {
    HeaderPublic,
    PublicFooters,
  },
};
</script>
<template>
  <HeaderPublic />
  <div>
    <div class="dropdown">
  <a class="btn btn-secondary dropdown-toggle" href="#" role="button" id="dropdownMenuLink" data-bs-toggle="dropdown" aria-expanded="false">
    Dropdown link
  </a>

  <ul class="dropdown-menu" aria-labelledby="dropdownMenuLink">
    <li><a class="dropdown-item" href="#">Action</a></li>
    <li><a class="dropdown-item" href="#">Another action</a></li>
    <li><a class="dropdown-item" href="#">Something else here</a></li>
  </ul>
</div>
  </div>
 <main>
  <p class="title text-center">Dịch vụ</p>
        <div class="">
          <div class="row text-center all-services">
            <div
              class="col rounded border border-dark container-icon col bg-cat_health_service kind-service"
            >
              <p class="icon-highligh">
                <i class="fa-solid fa-syringe icon-click"></i>
              </p>

              <h4><b>Physical examination</b></h4>
              <router-link class="" :to="{ name: 'PhysicalExamination' }"
                ><img
                  class="col-5 d-flex justify-content-center offset-4"
                  src="../../assets/images/cat_health_service1.jpg"
                  width="100px"
                  alt=""
              /></router-link>

              <p>Click to see more details!</p>
            </div>
            <div
              class="col rounded border border-dark container-icon col bg-cat_shower_service kind-service"
            >
              <p class="icon-highligh">
                <i class="fa-solid fa-shower icon-click"></i>
              </p>

              <h4><b>Spa- grooming</b></h4>
              <router-link class="" :to="{ name: 'SpaRoom' }"
                ><img
                  class="col-5 d-flex justify-content-center offset-4"
                  src="../../assets/images/cat_shower_service.jpg"
                  width="100px"
                  alt=""
              /></router-link>
              <p>Click to see more details!</p>
            </div>
            <div
              class="col rounded border border-dark container-icon col bg-cat-service-hotel kind-service"
            >
              <p class="icon-highligh">
                <i class="fa-solid fa-hotel icon-click"></i>
              </p>

              <h4><b>Hotel- service</b></h4>

              <router-link class="" :to="{ name: 'HotelRoom' }"
                ><img
                  class="col-5 d-flex justify-content-center offset-4 cat-service-hotel"
                  src="../../assets/images/cat_hotel_service.jpg"
                  width=""
                  alt=""
              /></router-link>

              <p>Click to see more details!</p>
            </div>
          </div>
        </div>
 </main>
  <PublicFooters />
</template>

<style>
@import "./Service.module.css";
</style>
