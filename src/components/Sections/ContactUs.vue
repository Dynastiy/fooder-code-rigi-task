<template>
  <div>
    <div class="contact-us">
      <div
        class="lg:tw-px-16 md:tw-px-12 tw-px-6 tw-flex tw-items-centern tw-justify-center tw-py-16"
      >
        <div
          class="tw-bg-white/10 tw-backdrop-blur tw-p-8 lg:tw-w-3/5 md:tw-w-4/5 tw-w-full tw-rounded-xl"
        >
          <h4 class="tw-text-3xl tw-mb-6 tw-text-white tw-font-bold tw-text-right">
            Contact us
          </h4>
          <form action="">
            <input type="text" placeholder="name" />
            <input type="email" placeholder="email" />
            <textarea
              name=""
              placeholder="message"
              id=""
              cols="30"
              rows="4"
            ></textarea>
            <div class="tw-text-center tw-mt-4">
                <button class="main-btn main-btn-primary">submit</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.contact-us {
  background-image: url("https://img.freepik.com/free-photo/spices-tomatoes-near-spaghetti-garlic_23-2147849739.jpg");
  background-blend-mode: overlay;
  /* min-height: 400px; */
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  /* background-attachment: fixed; */
}

form {
  display: flex;
  display: -ms-flexbox;
  display: inline-flex;
  flex-direction: column;
  gap: 20px;
  width: 100%;
}

input,
textarea {
  width: 100%;
  padding: 10px 20px !important;
  background: white;
  border: none;
  outline: none;
  /* border: 1px solid white; */
}

input::placeholder, textarea::placeholder {
    font-size: 13px;
    font-weight: 400 !important;
    color: var(--gray-600);
}
</style>
