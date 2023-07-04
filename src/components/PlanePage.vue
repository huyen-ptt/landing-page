<template>
  <div class="plane" id="pricing">
    <div class="title-plane">
      <div class="title-plane-big">Choose your plan</div>
      <div class="title-plane-small">Lorem ipsum dolor sit amet consectetur. Quis tortor gravida nibh arcu id
        <br>purus ullamcorper. Vel vel erat semper augue.
      </div>
    </div>
    <div class="wrapper-chose">
      <div class="item-chose">
       <div class="bao-item-chose">
         <div class="criteria">
           <img  class="premium"  src="@/assets/imgs/premium.png"/>
           <div class="package">Free</div>
           <div class="inherit">
             <div class="item-featuress">
               <img src="@/assets/imgs/tick-circle.png"/>
               <div>Unlimited bandwitch</div>
             </div>
             <div class="item-featuress">
               <img src="@/assets/imgs/tick-circle.png"/>
               <div>Encrypted connection</div>
             </div>
             <div class="item-featuress">
               <img src="@/assets/imgs/tick-circle.png"/>
               <div>Yes trafic logs</div>
             </div>
           </div>
         </div>
         <div class="price">Free</div>
       </div>
        <button class="btn-select">
          Select
        </button>
      </div>
      <div class="item-chose">
       <div class="bao-item-chose">
        <div class="criteria">
          <img class="premium" src="@/assets/imgs/premium.png"/>
          <div class="package">Standard plan</div>
          <div class="inherit">
            <div class="item-featuress">
              <img src="@/assets/imgs/tick-circle.png"/>
              <div>Unlimited bandwitch</div>
            </div>
            <div class="item-featuress">
              <img src="@/assets/imgs/tick-circle.png"/>
              <div>Encrypted connection</div>
            </div>
            <div class="item-featuress">
              <img src="@/assets/imgs/tick-circle.png"/>
              <div>Yes trafic logs</div>
            </div>
            <div class="item-featuress">
              <img src="@/assets/imgs/tick-circle.png"/>
              <div>Works on all devices</div>
            </div>
            <div class="item-featuress">
              <img src="@/assets/imgs/tick-circle.png"/>
              <div>Connect anyware</div>
            </div>
          </div>
        </div>
         <div class="price">$ 9 / <span>mo</span></div>
       </div>
        <button class="btn-select">
          Select
        </button>
      </div>
      <div class="item-chose">
        <div class="bao-item-chose">
          <div class="criteria">
            <img class="premium" src="@/assets/imgs/premium.png"/>
            <div class="package">Premium plan</div>
            <div class="inherit">
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Unlimited bandwitch</div>
              </div>
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Encrypted connection</div>
              </div>
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Yes trafic logs</div>
              </div>
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Works on all devices</div>
              </div>
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Connect anyware</div>
              </div>
              <div class="item-featuress">
                <img src="@/assets/imgs/tick-circle.png"/>
                <div>Get new features</div>
              </div>
            </div>
          </div>
          <div class="price">$ 12 / <span>mo</span></div>
        </div>
        <button class="btn-select">
          Select
        </button>
      </div>
    </div>
  </div>
</template>
<style scoped lang="scss">
.plane{
  max-width: 1000px;
  margin: 0 auto;
  .title-plane{
    text-align: center;
    .title-plane-big{
      color: var(--gray, #2B2B2B);
      font-size: 30px;
      font-weight: 600;
      padding-bottom: 15px;
    }
    .title-plane-small{
      color: #5A5A5A;
      font-weight: 600;
      font-size: 16px;
      padding-bottom: 21px;
    }
  }
  .wrapper-chose{
    display: flex;
    justify-content: space-between;
    .item-chose{
      padding: 25px 65px;
      border-radius: 20px;
      border: 2px solid #D3D3D3;
      display: flex;
      justify-content: space-between;
      flex-direction: column;
      align-items: center;
      .premium{
        margin-bottom: 40px;
      }
      .package{
        margin-bottom: 55px;
        font-size: 20px;
        font-weight: 600;
      }
      .bao-item-chose{
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        align-items: center;
        .criteria{
          display: flex;
          justify-content: space-between;
          flex-direction: column;
          align-items: center;
        }
        .item-featuress{
          display: flex;
          gap:5px;
          align-items: center;
          padding-bottom: 40px;
        }
        .inherit{
          height: 385px;
        }
        .price{
          color: var(--gray, #2B2B2B);
          font-size: 28px;
          font-weight: 600;
          margin-bottom: 22px;
          span{
            color: #646464;
            font-size: 20px;
            font-weight: 400;
          }
        }
      }
      .btn-select{
        color: #FFF;
        font-size: 20px;
        font-weight: 500;
        border-radius: 20px;
        background: var(--red, #F53838);
        padding: 12px 50px;
        border: 0;
        &:hover{
          cursor: pointer;
          color: #2B2B2B;
          background: #FCAEAE;
          transition: 1s;
        }
      }
    }
  }
}
@media (max-width: 450px) {
  .plane{
    padding: 0 19px;
    .title-plane{
      .title-plane-big{
        font-size: 19px;
        padding-bottom: 10px;
      }
      .title-plane-small{
        font-size: 10px;
        padding-bottom: 18px;
      }
    }
    .wrapper-chose{
      gap:10px;
      overflow:hidden ;
      .item-chose{
        padding: 15px 30px;
        .btn-select{
          font-size: 13px;
        }
        .bao-item-chose{
          .item-featuress{
            padding-bottom: 30px;
          }
          .price{
            font-size: 16px;
            span{
              font-size: 10px;
            }
          }
        }
      }
    }
  }
}
</style>