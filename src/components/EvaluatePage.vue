<template>
  <div class="evaluate" id="testimonial">
    <div class="title-evaluate">
      <div class="title-evaluate-big">Trusted by thousands of<br>
        happy customer
      </div>
      <div class="title-evaluate-small">Lorem ipsum dolor sit amet consectetur. Quis tortor gravida nibh arcu<br> id
        purus ullamcorper. Vel vel erat semper augue.
      </div>
    </div>
    <div class="wrapper-evaluate">
      <div v-for="item in evaluateList" class="item-evaluate">
        <div class="person-evaluate">
          <img class="avt" :src="item.img"/>
          <div>
            <div class="name-person">{{item.name}}</div>
            <div class="local-person">
              <div>{{item.local}}</div>
              <div class="total-star">
                <div>{{item.star}}</div>
                <img src="@/assets/imgs/sao.png"/>
              </div>
            </div>
          </div>
        </div>
        <div class="content-cmt">{{item.contentRated}}
        </div>
      </div>
    </div>
    <div class="toolbar">
      <img class="frame" src="@/assets/imgs/frame.png"/>
      <div class="arrow">
        <img src="@/assets/imgs/arrow-circle-right.png"/>
        <img src="@/assets/imgs/arrow-circle-left.png"/>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      evaluateList: [
        {
          id: 1,
          img: 'https://images.unsplash.com/photo-1544005313-94ddf0286df2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1888&q=80',
          name: 'Brooklyn Simmons',
          local: 'Warsaw,pland',
          star: 4.5,
          contentRated: '“wow...iam very happy to use this vpn,it\n' +
              'turned out to be more than my expectations\n' +
              'and so far there have been no problems.\n' +
              'laslesvpn always the best”.'
        },
        {
          id: 2,
          img: 'https://plus.unsplash.com/premium_photo-1669741908308-5ca216f3fcd1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2069&q=80',
          name: 'Darlene Robertson',
          local: 'Warsaw,pland',
          star: 4.5,
          contentRated: '“wow...iam very happy to use this vpn,it\n' +
              'turned out to be more than my expectations\n' +
              'and so far there have been no problems.\n' +
              'laslesvpn always the best”.'
        },
        {
          id: 3,
          img: 'https://images.unsplash.com/photo-1554151228-14d9def656e4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1886&q=80',
          name: 'Darrell Steward',
          local: 'Warsaw,pland',
          star: 4.5,
          contentRated: '“wow...iam very happy to use this vpn,it\n' +
              'turned out to be more than my expectations\n' +
              'and so far there have been no problems.\n' +
              'laslesvpn always the best”.'
        },
      ]
    }
  }
}
</script>
<style scoped lang="scss">
.evaluate {
  padding-top: 8px;
  padding-bottom: 88px;
  max-width: 1200px;
  margin: 0 auto;

  .title-evaluate {
    .title-evaluate-big {
      color: var(--gray, #2B2B2B);
      text-align: center;
      font-size: 30px;
      font-weight: 600;
      padding-bottom: 12px;
    }

    .title-evaluate-small {
      color: #5A5A5A;
      text-align: center;
      font-size: 16px;
      font-weight: 400;
      padding-bottom: 20px;
    }
  }
  .wrapper-evaluate{
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap:18px;
    margin-bottom: 27px;
    .item-evaluate{
      border-radius: 20px;
      border: 1px solid #CCC;
      padding: 38px;
      &:hover{
        border: 1px solid var(--red, #F53838);
        cursor: pointer;
      }
      .avt{
        width: 64px;
        height: 64px;
        border-radius: 999px;
        object-fit: cover;
      }
      .person-evaluate{
        display: flex;
        align-items: center;
        gap:28px;
        margin-bottom: 21px;
        .name-person{
          color: #2C2C2C;
          font-size: 18px;
          font-weight: 600;
        }
        .local-person{
          display: flex;
          align-items: center;
          color: #7B7B7B;
          font-size: 15px;
          font-weight: 400;
          //justify-content: space-between;
          gap:80px;
          .total-star{
            display: flex;
            align-items: center;
            font-weight: 500;
            gap:5px;
          }
        }
      }
      .content-cmt{
        color: #5A5A5A;
        font-size: 16px;
        font-weight: 400;
      }
    }
  }
  .toolbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .arrow{
      display: flex;
      align-items: center;
      gap:42px;
      cursor: pointer;
      &:hover{
        //color: #F53838;
      }
    }
  }
}
@media (max-width: 600px) {
  .evaluate{
    padding:40px 19px;
    .toolbar{
      .frame{
        width: 70px;
      }
      .arrow{
        img{
          width: 30px;
        }
      }
    }
    .title-evaluate{
      .title-evaluate-big{
        font-size: 17px;
      }
      .title-evaluate-small{
        font-size: 9px;
        padding-bottom: 38px;
      }
    }
    .wrapper-evaluate{
      overflow: hidden;
      .item-evaluate{
        padding: 20px;
        .content-cmt{
          font-size: 11px;
        }
        .person-evaluate{
          gap:20px;
          .avt{
            width: 40px;
            height: 40px;
          }
          .name-person{
            font-size: 11px;
          }
          .local-person{
            font-size: 9px;
          }
        }
      }

    }
  }
}

</style>