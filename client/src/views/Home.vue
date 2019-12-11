<template>
  <main>
    <div class="home">
      <p>Online library for university students</p>
      <p class="details">
        We build put together academic resources that empower students and
        connect them to solutions that enable productivity, growth, and
        discovery.
      </p>
      <div class="button-holder">
        <a href="#slider-image-1" class="dots"></a>
        <a href="#slider-image-1" class="dots"></a>
        <a href="#slider-image-1" class="dots"></a>
      </div>
    </div>

    <section class="about-edutec">
      <div class="container">
        <div class="about-content">
          <p>About Edutec</p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Exercitationem, illo. Consequuntur, doloremque quos delectus,
            similique praesentium distinctio facere provident quia dolorem dolor
            accusantium, reprehenderit voluptatem numquam soluta tempora unde
            explicabo laboriosam corrupti. Eaque sint esse facere nesciunt,
            alias voluptas labore excepturi aperiam laboriosam a ipsum quasi
            quam, temporibus velit! Animi aliquid accusamus, culpa ipsum odit
            neque error! Sit ipsum amet beatae ipsam! Officia laudantium laborum
            asperiores.
          </p>
        </div>
      </div>
    </section>

    <section class="services">
      <div class="service">
        <div class="serve">
          <p>Services</p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Accusantium beatae quis tenetur cumque provident quidem tempora
            natus animi mollitia
          </p>
        </div>

        
      </div>
    </section>

    <section class="category">
      <div class="books">
        <div class="category-circle">
          <div class="circle">
            <p>200</p>
            <p>Category</p>
          </div>
          <div class="circle">
            <p>900k</p>
            <p>Users</p>
          </div>
          <div class="circle">
            <p>9k</p>
            <p>Academic Questions</p>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  components: {}
};
</script>

<style lang="scss" scoped>
.home {
  background: linear-gradient(
      135deg,
      rgba(13, 13, 14, 0.4) 0%,
      rgba(10, 10, 10, 0.6) 100%
    ),
    url('https://images.pexels.com/photos/590493/pexels-photo-590493.jpeg')
      no-repeat center center / cover;
  width: 100%;
  height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  font-family: Avenir, sans-serif;
  p {
    &:first-child {
      font-size: 14px;
      width: 233px;
      height: 19.56px;
      color: #ffffff;
    }
    &:nth-child(2) {
      color: white;
      text-align: center;
      font-size: 46px;
      max-width: 62.5rem;
      width: 100%;
      height: 15.445rem;
      line-height: 3.75rem;
      font-weight: 900;
      font-style: normal;
    }
  }
  .button-holder {
    position: absolute;
    bottom: 0;
    left: 45%;
    .dots {
      display: inline-block;
      height: 15px;
      width: 15px;
      background: #828282;
      margin: 0.4rem 0.3rem;
      border-radius: 3rem;
      &:first-child {
        background: #e17a4e;
      }
    }
  }
}

.container {
  max-width: 62.5rem;
  margin: 0 auto;
  width: 100%;
  padding: 0 1.5rem;
  .about-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 1.5rem 0;
    font-family: Avenir, sans-serif;
    p {
      &:first-child {
        color: #1a757b;
        line-height: 41px;
        font-size: 1.875rem;
        font-weight: 500;
      }
      &:nth-child(2) {
        color: #797979;
        mix-blend-mode: normal;
        opacity: 0.81;
        line-height: 25px;
        font-size: 1.125rem;
        font-weight: normal;
        font-style: normal;
        text-align: center;
      }
    }
  }
}

.services {
  background: #f2efdf;
  .service {
    display: flex;
    .serve {
      max-width: 935px;
      width: 100%;
      margin: 0 auto;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 20px;
      p {
        &:first-child {
          color: #1a757b;
          margin-top: 30px;
          font-size: 30px;
          font-style: medium;
          line-height: 40.98px;
        }
        &:last-child {
          text-align: center;
          color: #797979;
          opacity: 81.43%;
          font-size: 18px;
        }
      }
    }
  }
}

.books {
  background: linear-gradient(to bottom, rgba(26, 117, 123, 0.55)),
    url('https://images.pexels.com/photos/1005324/literature-book-open-pages-1005324.jpeg')
      no-repeat center center / cover;
  height: 235px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  .category-circle {
    display: -webkit-box;
    .circle {
      color: white;
      margin: 0 4.5rem;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      p {
        &:first-child {
          width: 54px;
          height: 54px;
          border-radius: 50%;
          background: white;
          text-align: center;
          color: #797979;
        }
      }
    }
  }
}
</style>
