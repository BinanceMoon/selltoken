<template>
  <div class="page-index">
    <!-- 背景 -->
    <video muted loop class="video-bg" autoplay playsinline>
      <source src="/videos/IMG_6322228.MP4" type="video/mp4" />
    </video>
    <!-- 顶部 -->
    <div class="container">
      <!-- 标题 -->
      <div class="page-title">
        <h1>{{ $t('PageHome.text1') }}</h1>
        <h2><span v-html="$t('PageHome.text2')"></span></h2>
        <div class="home-landing-animation-cover" @click="initRenderCharts">
          <svg width="100%" height="100%" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" baseProfile="full" viewBox="0 0 510 510">
            <rect width="510" height="510" x="0" y="0" id="0" fill="none" fill-opacity="1"></rect>
            <path d="M255 25.9A20 20 0 0 1 276.7 5.9A250 250 0 0 1 496.5 190.3A20 20 0 0 1 480.6 215.2L308.9 245.5A5 5 0 0 1 303.2 241.9A50 50 0 0 0 259.5 205.2A5 5 0 0 1 255 200.2Z" fill="#5470c6" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-0"></path>
            <path d="M443.3 221.8A18 18 0 0 1 464.3 238.1A210 210 0 0 1 393.8 412.6A18 18 0 0 1 367.4 409.6L287.2 299.3A5 5 0 0 1 287.9 292.6A50 50 0 0 0 304.8 250.8A5 5 0 0 1 308.9 245.5Z" fill="#91cc75" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-1"></path>
            <path d="M356.8 395.2A16 16 0 0 1 352.1 418.3A190 190 0 0 1 206.7 438.8A16 16 0 0 1 195.7 417.8L236.3 306.5A5 5 0 0 1 242.2 303.3A50 50 0 0 0 280.6 298A5 5 0 0 1 287.2 299.3Z" fill="#fac858" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-2"></path>
            <path d="M201.9 401A14 14 0 0 1 182.8 408.9A170 170 0 0 1 103.7 332.6A14 14 0 0 1 110.9 313.2L204.2 275.5A5 5 0 0 1 210.5 277.9A50 50 0 0 0 233.7 300.2A5 5 0 0 1 236.3 306.5Z" fill="#ee6666" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-3"></path>
            <path d="M132.2 304.6A12 12 0 0 1 116.2 297A145 145 0 0 1 112.6 227.8A12 12 0 0 1 127.7 218.5L202.3 239.9A5 5 0 0 1 205.9 245.6A50 50 0 0 0 207.1 269.4A5 5 0 0 1 204.2 275.5Z" fill="#73c0de" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-4"></path>
            <path d="M144.9 223.4A10 10 0 0 1 138.3 210.2A125 125 0 0 1 160.7 173A10 10 0 0 1 175.4 172.6L217 215.6A5 5 0 0 1 217.1 222.3A50 50 0 0 0 208.4 236.9A5 5 0 0 1 202.3 239.9Z" fill="#3ba272" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-5"></path>
            <path d="M184.4 181.9A8 8 0 0 1 185 170.1A110 110 0 0 1 209.4 154.9A8 8 0 0 1 220.2 159.4L236.3 203.5A5 5 0 0 1 233.7 209.8A50 50 0 0 0 223.7 216A5 5 0 0 1 217 215.6Z" fill="#fc8452" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-6"></path>
            <path d="M222.9 166.8A6 6 0 0 1 226.9 159A100 100 0 0 1 248.6 155.2A6 6 0 0 1 255 161.2L255 200.2A5 5 0 0 1 250.5 205.2A50 50 0 0 0 242.2 206.7A5 5 0 0 1 236.3 203.5Z" fill="#9a60b4" stroke="white" stroke-width="4" stroke-linejoin="round" transform-origin="255px 255px" class="zr0-cls-7"></path>
          </svg>
          <div id="play-landing-animation">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z" clip-rule="evenodd"></path>
            </svg>
          </div>
        </div>
      </div>
      <!-- 操作池 -->
      <div class="operation-pool">
        <div class="pool-aintext">
          <el-button type="text" @click="toRoute('https://app.selltoken.org/#/swap')">{{ $t('PageHeader.Swap') }}</el-button>
          <el-button type="text" @click="toRoute('/miner')">{{ $t('PageHeader.Miner') }}</el-button>
          <el-button type="text" @click="toRoute('/liquidity')">{{ $t('PageHeader.Liquidity') }}</el-button>
        </div>
        <auto-search @select="onSelectCoinbase" @clear="onClearSelectInfo"
          :content="$t('new03.text1')"></auto-search>
        <h3 class="pair-h3">{{ $t('PageHome.text3') }}</h3>
        <div class="pair-content">
          <div class="unitem" 
            v-for="(item, index) in pairLists" :key="index"
            :class="{active: selectPairIndex === index}" >
            <img :src="require(`~/static/images/${item}.png`)" alt="">
            <span>{{ item }}</span>
          </div>
        </div>
        <div class="no-pair">
          <span v-if="selectInfo && selectPairIndex<0">{{ $t('noPair') }}</span>
        </div>
        <!-- 输入BNB -->
        <div class="write-amount">
          <el-input-number 
            v-model="amountNumber" controls-position="right" 
            :min="0.0000001" :step="0.1">
          </el-input-number>
          <div class="amount-unit">
            <img src="~/static/images/BNB.png" alt="" class="unitico">
            <span>{{ $t('PageHome.text26') }}</span>
          </div>
        </div>
        <div class="slider-linebox">
          <el-slider v-model="sliderLineValue" :min="25" :step="25" show-stops :marks="sliderMarks"
            @change="onChangeSlider"></el-slider>
        </div>
        <div class="max-short">
          <p>
            {{ $t('PageHome.text4') }}:
            <b>{{ maxAmountShort }}</b>
            <i v-if="queryMaxLoading" class="el-icon-loading"></i>
            BNB</p>
        </div>
        <div class="shortbtn-cell">
          <el-button 
            :disabled="!addr2Token||!selectInfo||selectInfo.pairs=='No pair'"
            @click="onOpenShort">
            {{ $t('PageHome.text5') }}
          </el-button>
          <el-button class="btncolor2" @click="toLiquidity"
            :disabled="!selectInfo">
            {{ $t('PageHome.text6') }}
          </el-button>
        </div>
      </div>
      <!-- 奖池 -->
      <div class="jackpot-box">
        <div class="jack-item">
          <div class="j-radius"></div>
          <div class="j-title">
            <h6>{{ $t('PageHome.text7') }}</h6>
          </div>
          <div class="j-amount">
            <p>
              <img src="~/static/images/BNB.png" alt="" class="j-unit">
              <b>{{ shortsInfos[1] || '0.00000000' }}</b>
            </p>
          </div>
          <img src="~/static/images/v1.png" alt="" class="j-ico">
        </div>
        <div class="jack-item">
          <div class="j-radius"></div>
          <div class="j-title">
            <h6>{{ $t('PageHome.text5') }}</h6>
          </div>
          <div class="j-amount">
            <p>
              <img src="~/static/images/BNB.png" alt="" class="j-unit">
              <b>{{ shortsInfos[0] || '0.00000000' }}</b>
            </p>
          </div>
          <img src="~/static/images/v2.png" alt="" class="j-ico">
        </div>
        <div class="jack-item">
          <div class="j-radius"></div>
          <div class="j-title">
            <h6>{{ $t('PageHome.text6') }}</h6>
          </div>
          <div class="j-amount">
            <p class="size-text">
              {{ $t('PageHome.text8') }}：
              <img :src="coinbaseIcos[selectInfo?selectInfo.name:'']||require('~/static/images/defaultico.png')" alt="" class="j-unit">
              <b>{{ shortsInfos[2] || '0.0000' }}</b>
            </p>
            <p class="size-text">
              {{ $t('PageHome.text9') }}：
              <img :src="coinbaseIcos[selectInfo?selectInfo.name:'']||require('~/static/images/defaultico.png')" alt="" class="j-unit">
              <b>{{ shortsInfos[3] || '0.0000' }}</b>
            </p>
            <p class="size-text">
              {{ $t('PageHome.text10') }}：
              <b>{{ (((shortsInfos[3]/shortsInfos[2])*100)||0).toFixed(2) }}%</b>
            </p>
          </div>
          <img src="~/static/images/v3.png" alt="" class="j-ico">
        </div>
      </div>
    </div>
    <!-- 订单 -->
    <div class="orderinfo-box">
      <div class="swiper-orderinfo" v-swiper:mySwiper="SwiperOptions">
        <div class="swiper-wrapper">
          <div class="swiper-slide" v-for="(item, index) in myOrderLists" :key="index">
            <div class="orderinfo-item">
              <img src="~/static/images/vinitembg.png" alt="" class="vimg-bg">
              <div class="coin-colors"
                :style="{backgroundColor: item[2]-item[1]>=0 ? '#48c774' : 'red'}"></div>
              <div class="o-top">
                <div class="ot-logo">
                  <img :src="coinbaseIcos[item[3]]||require('~/static/images/defaultico.png')" alt="">
                </div>
                <strong>{{ $t('new01.text1') }}</strong>
                <div class="o-types">
                  <b>{{ $t('new01.text2') }}</b>
                  <span v-if="item[4] != 'No pair'">{{ item[4] }}/{{ item[3] }}</span>
                  <span v-else>{{ item[4] }}</span>
                </div>
              </div>
              <div class="o-info">
                <div class="o-addr">
                  <div class="o-tag">{{ $t('new01.text3') }}</div>
                  <span>{{ item[0].substr(0, 4) }}...{{ item[0].substr(-6) }}</span>
                  <img src="~/static/images/copyico.png" alt="" class="copybtn"
                    @click="onCopyText(item[0])">
                </div>
                <div class="oflex-cell">
                  <div class="o-price">
                    $
                    {{ item[5] }}
                  </div>
                  <div class="o-rate">
                    <span :style="{color: item[2]-item[1]>=0 ? '#48c774' : 'red'}"
                      v-if="item[2]!=0">
                      {{ item[2]-item[1]>=0 ? '+' : '' }}
                      {{ (item[2]/item[1]*100-100).toFixed(2) }}%
                    </span>
                    <span v-else>
                      0.00%
                    </span>
                  </div>
                </div>
                <div class="o-cellitem">
                  <span>{{ $t('new01.text4') }}</span>
                  <i class="oline"></i>
                  <strong>
                    <img src="~/static/images/BNB.png" class="sico" />
                    {{ item[1] }}
                  </strong>
                </div>
                <div class="o-cellitem">
                  <span>{{ $t('new01.text5') }}</span>
                  <i class="oline"></i>
                  <strong>
                    <img src="~/static/images/BNB.png" class="sico" />
                    {{ item[2] }}
                  </strong>
                </div>
                <div class="cp-btnbox">
                  <div class="inbtntext" :class="{disabled: item[0]==0}" @click="onClosePostion(item[0])">
                    <span>{{ $t('PageHome.text7') }}</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
    <!-- mind map -->
    <div class="mindmap-video">
      <video muted loop width="100%" style="margin:auto;" autoplay playsinline>
        <source :src="`/lang/videos/${$i18n.locale}.mp4`" type="video/mp4">
      </video>
      <img :src="`/lang/images/${$i18n.locale}.png`" alt="" class="flow-img">
    </div>
    <!-- IDO -->
    <div class="ido-content">
      <h2>SeIIToKen IDO</h2>
      <div class="container">
        <div class="disc-box">
          <div class="timecount-statistic">
            <!-- <el-statistic :value="deadline3" time-indices
              format="DD [day] HH [hour] mm [minute] ss [second]" :value-style="valueStyle">
              <span slot="prefix">Distance End</span>
            </el-statistic> -->
            <span>{{ $t('PageHome.text16') }}</span>
            <b>00</b>
            <span>{{ $t('PageHome.text17') }}</span>
            <b>00</b>
            <span>{{ $t('PageHome.text18') }}</span>
            <b>00</b>
            <span>{{ $t('PageHome.text19') }}</span>
            <b>00</b>
            <span>{{ $t('PageHome.text20') }}</span>
          </div>
          <div class="sline">
            <div class="slineitem"></div>
          </div>
          <div class="disc-join">
            <el-input-number :controls="false" placeholder="BNB Value"></el-input-number>
            <el-button type="primary" disabled>{{ $t('PageHome.text21') }}</el-button>
          </div>
        </div>
      </div>
    </div>
    <!-- dife link -->
    <div class="dife-linkbox">
      <div class="container">
        <div class="dife-info">
          <h3 v-html="$t('PageHome.text22')"></h3>
          <p>{{ $t('PageHome.text23') }}</p>
        </div>
      </div>
      <div class="link-logo">
        <ul class="link-line-item">
          <li
            v-for="(item, index) in aLinkItem1" :key="index">
            <img :src="item.icon" alt="">
            <span>{{ item.name }}</span>
          </li>
        </ul>
        <ul class="link-line-item linitem2">
          <li
            v-for="(item, index) in aLinkItem2" :key="index">
            <img :src="item.icon" alt="">
            <span>{{ item.name }}</span>
          </li>
        </ul>
      </div>
    </div>
    <!-- charts -->
    <el-dialog
      :visible.sync="showChartsModal"
      width="500px"
      custom-class="customCharts-dialog">
      <div id="modalCharts" class="charts-box"></div>
    </el-dialog>
    <!-- charts modal -->
    <el-dialog
      width="600px"
      :visible.sync="showChartsModalInfo"
      center
      custom-class="customCharts-info">
      <div slot="title" class="charts-modal-title">
        <h2>
          <img src="~/static/images/vnotice1.png" />
          {{ $t('new03.text4') }}
        </h2>
      </div>
      <div class="charts-modal-content">
        <div class="prxin">
          <h3>{{ $t('new03.text5') }}</h3>
          <p>
            {{ $t('new03.text6') }} <br>
            {{ $t('new03.text7') }} <br>
            {{ $t('new03.text8') }} <br>
            {{ $t('new03.text9') }}
          </p>
        </div>
        <h3>{{ $t('new03.text10') }}</h3>
        <p>
          1、{{ $t('new03.text11') }} <br>
          2、{{ $t('new03.text12') }} <br>
        </p>
        <h3>{{ $t('new03.text13') }}</h3>
        <p>1、{{ $t('new03.text14') }}</p>
        <div class="charts-foot-address">
          <span>{{ $t('new03.text15') }}</span>
          <b>0xa645995e9801f2ca6e2361edf4c2a138362bade4</b>
          <img src="~/static/images/copyico.png" 
            @click="onCopyText('0xa645995e9801f2ca6e2361edf4c2a138362bade4')" />
        </div>
        <div class="charts-fixed-right">
          <strong>5%</strong>
          <small>{{ $t('new03.text16') }}</small>
        </div>
      </div>
    </el-dialog>
  </div>
</template>

<script>
import { BNB_ADDRESS, USDT_ADDRESS } from '@/contract/ABI';
import * as echarts from 'echarts';
export default {
  name: 'IndexPage',
  data () {
    return {
      initCharts: false,
      showChartsModalInfo: false,
      nowSelectChartsInfo: {},
      showChartsModal: false,
      sliderMarks: {
        0: '0%',
        25: '25%',
        50: '50%',
        75: '75%',
       100: '100%',
      },
      sliderLineValue: 0,
      aLinkItem1: [
        {
          icon: require('~/static/images/Arbitrum.svg'),
          name: 'Arbitrum'
        },
        {
          icon: require('~/static/images/Avalanche.svg'),
          name: 'Avalanche'
        },
        {
          icon: require('~/static/images/Binance.svg'),
          name: 'Binance'
        },
        {
          icon: require('~/static/images/Ethereum.svg'),
          name: 'Ethereum'
        },
        {
          icon: require('~/static/images/Solana.svg'),
          name: 'Solana'
        },
        {
          icon: require('~/static/images/Fandom.svg'),
          name: 'Fantom'
        }
      ],
      aLinkItem2: [
        {
          icon: require('~/static/images/Moonbeam.svg'),
          name: 'Moonbeam'
        },
        {
          icon: require('~/static/images/Near.svg'),
          name: 'Near'
        },
        {
          icon: require('~/static/images/Nervos.svg'),
          name: 'Nervos'
        },
        {
          icon: require('~/static/images/Optimism.svg'),
          name: 'Optimism'
        },
        {
          icon: require('~/static/images/Polygon.svg'),
          name: 'Polygon'
        },
        {
          icon: require('~/static/images/Harmony.svg'),
          name: 'Harmony'
        },
        {
          icon: require('~/static/images/Iotex.svg'),
          name: 'IoTeX'
        }
      ],
      pairLists: ['BNB', 'USDT'],
      deadline3: Date.now() + 1000 * 1000 * 60 * 30,
      SwiperOptions: {
        slidesPerView: 5,
        spaceBetween: 30,
        slidesPerGroup: 1,
        loop: false,
        loopFillGroupWithBlank: false,
        autoplay: false,
        breakpoints: {
          1920: {
            slidesPerView: 4,
            spaceBetween: 30,
            slidesPerGroup: 1,
          },
          1440: {
            slidesPerView: 3,
            spaceBetween: 20,
            slidesPerGroup: 1,
          },
          1080: {
            slidesPerView: 2,
            spaceBetween: 30,
            slidesPerGroup: 1,
          },
          750: {
            slidesPerView: 1,
            spaceBetween: 30,
            slidesPerGroup: 1,
          },
          300: {
            slidesPerView: 1,
            spaceBetween: 10,
            slidesPerGroup: 1,
          }
        },
        navigation: {
          nextEl: '.orderinfo-box .swiper-button-next',
          prevEl: '.orderinfo-box .swiper-button-prev',
        }
      },
      selectValue: '',
      selectInfo: null,
      selectPairIndex: -1,
      amountNumber: 0.1,
      shortsInfos: {},
      miningUserInfos: {},
      commonAddrs: {
        'BNB': BNB_ADDRESS,
        'USDT': USDT_ADDRESS
      },
      maxAmountShort: '0.00000000',
      myOrderLists: [
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: 'No pair'
        },
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: 'No pair'
        },
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: 'No pair'
        },
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: 'No pair'
        },
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: 'No pair'
        },
        {
          0: '0x0000000000000000000000000000000000000000',
          1: '0.00000000',
          2: '0.00000000',
          3: '',
          4: ''
        }
      ],
      queryMaxLoading: false,
      timers: {0:null, 1:null}, // 定时器
    }
  },
  computed: {
    addr2Token () {
      return this.commonAddrs[this.pairLists[this.selectPairIndex]];
    },
    coinbaseIcos () {
      return this.$store.state.coinbaseIcos;
    },
    walletAddress () {
      return this.$store.state.wallet.walletAddress;
    },
  },
  created () {
    this.queryMyOrderSell()
  },
  destroyed () {
    for (let k in this.timers) {
      clearTimeout(this.timers[k])
      clearInterval(this.timers[k])
    }
  },
  mounted () {
  },
  methods: {
    toRoute (url) {
      if (url.startsWith('http')) {
        window.open(url)
      } else {
        this.$router.push(this.localePath(url))
      }
    },
    async initRenderCharts () {
      this.showChartsModal = true
      if (this.initCharts) return false;
      const option = {
        title: {
          text: this.$t('new03.text17'),
          subtext: 'Fake Data',
          left: 'center',
          textStyle: {
            color: '#ffffff',
            fontSize: 28,
          }
        },
        legend: {
          orient: 'horizontal',
          left: 'center',
          bottom: 20,
          textStyle: {
            color: '#fff'
          }
        },
        tooltip: {
          formatter: function (item) {
            return `
              <div style="display:flex;align-items:center; margin-bottom:10px;">
                <i style="width:8px;height:8px;border-radius:50%;background:${item.color}"></i>
              </div>
              <span style="margin-right:10px;">${item.name}：</span>
              <b style="color:${item.color}">${item.value}%</b>
            `;
          },
          trigger: 'item'
        },
        series: [
          {
            name: this.$t('new03.text17'),
            type: 'pie',
            radius: '50%',
            label: {
              color: '#ffffff'
            },
            data: [
              { value: 10, name: 'Short liquidity' },
              { value: 5, name: 'air-drop' },
              { value: 40, name: 'LP  liquidity' },
              { value: 40, name: 'IDO' },
              { value: 5, name: 'Team' }
            ],
            emphasis: {
              itemStyle: {
                shadowBlur: 10,
                shadowOffsetX: 0,
                shadowColor: 'rgba(0, 0, 0, 0.5)'
              }
            }
          }
        ]
      };
      this.$nextTick(() => {
        this.initCharts = true
        const myChart = echarts.init(document.getElementById('modalCharts'));
        myChart.setOption(option);
        myChart.on('click', (params) => {
          this.showChartsModalInfo = true;
          // this.nowSelectChartsInfo = params.data;
        });
      })
    },
    onChangeSlider () {
      let num = Number(this.maxAmountShort)*this.sliderLineValue/100;
      if (num < 0.0000001) num = 0.1;
      this.amountNumber = num;
    },
    onCopyText (text) {
      this.$copyText(text).then((e) => {
        console.log(e)
        this.$message.success(this.$t('copySuccess'))
      }, () => {
        this.$message.success(this.$t('copyFail'))
      })
    },
    onClearSelectInfo () {
      this.selectInfo = null;
      this.selectPairIndex = -1;
      this.maxAmountShort = '0.00000000';
    },
    onSelectCoinbase (item) {
      this.selectInfo = item;
      this.selectValue = item.addr;
      this.selectPairIndex = this.pairLists.indexOf(item.pairs)
      this.queryShorts()
      this.queryMaxShorts()
      clearInterval(this.timers[1])
      this.timers[1] = setInterval(() => {
        this.queryMaxShorts()
        this.queryShorts()
      }, 10 * 1000)
    },
    async queryCoinbasePrice (index, pairName) {
      const { methods } = await this.$store.dispatch('contract/event');
      let addr1 = this.myOrderLists[index][0];
      let addr2 = this.commonAddrs[pairName];
      console.log(addr1, addr2)
      methods.getToken3Price(addr1, addr2).call((err, res) => {
        if (!err) {
          this.$set(this.myOrderLists[index], 5, (res/Math.pow(10, 18)).toFixed(8))
        }
      })
    },
    async onClosePostion (addr) {
      const { methods } = await this.$store.dispatch('contract/event');
      if (addr == 0) return false;
      methods.withdraw(addr).send((err, txHash) => {
        if (!err) {
          this.$store.dispatch('contract/cochainHashSuccess', { txHash })
        } else {
          this.$store.dispatch('contract/cochainHashError', { err })
        }
      })
    },
    async queryMyOrderSell () {
      const { methods } = await this.$store.dispatch('contract/event');
      methods.getMyPriceSell(this.walletAddress).call((err, res) => {
        if (!err) {
          if (res[0].length) {
            this.myOrderLists = res[0].map((addr, index) => {
              methods.getToke(addr).call((err, res) => {
                if (!err) {
                  this.myOrderLists[index][3] = res[0];
                  this.myOrderLists[index][4] = res[1];
                  this.queryCoinbasePrice(index, res[1])
                }
              })
              return {
                0: addr,
                1: (res[1][index]/Math.pow(10,18)).toFixed(8),
                2: (res[2][index]/Math.pow(10,18)).toFixed(8),
                3: '',
                4: '',
                5: ''
              }
            })
          }
          // 查询
          this.timers[0] = setTimeout(this.queryMyOrderSell, 10 * 1000);
        }
      })
    },
    async onOpenShort () {
      // 校验金额是否超过max
      if (this.amountNumber > this.maxAmountShort) {
        this.$alert(
          this.$t('PageHome.text4') + ' ' + this.maxAmountShort + ' BNB', 
          this.$t('PageHome.text27'), 
          {
            confirmButtonText: this.$t('PageHome.text29'),
            type: 'warning'
        })
        return false;
      }
      // 校验钱包余额不足
      const walletAmount = await this.$store.dispatch('wallet/queryAmountBNB');
      if (walletAmount < this.amountNumber) {
        return this.$message.warning(this.$t('new02.text7'));
      }
      // 执行操作
      const { methods } = await this.$store.dispatch('contract/event');
      const amount = web3.utils.toWei(String(this.amountNumber), 'ether');
      methods.ShortStart(this.selectValue, this.walletAddress, 100).send({
        value: amount
      },(err, txHash) => {
        if (!err) {
          this.$store.dispatch('contract/cochainHashSuccess', { txHash })
        } else {
          this.$store.dispatch('contract/cochainHashError', { err })
        }
      })
    },
    toLiquidity () {
      const addr1 = this.selectValue;
      const addr2 = this.addr2Token;
      this.$router.push({
        path: this.localePath('/liquidity'),
        query: {
          addr1, addr2
        }
      })
    },
    async queryShorts () {
      const { methods } = await this.$store.dispatch('contract/event');
      methods.getShorts(this.selectValue).call((err, res) => {
        if (!err) {
          console.log(res)
          this.shortsInfos = {
            0: (res[0]/Math.pow(10,18)).toFixed(8),
            1: (res[1]/Math.pow(10,18)).toFixed(8),
            2: (res[2]/Math.pow(10,18)).toFixed(4),
            3: (res[3]/Math.pow(10,18)).toFixed(4),
          }
        }
      })
    },
    async queryMaxShorts () {
      const { methods } = await this.$store.dispatch('contract/event');
      // 查询最大做空
      console.log(this.addr2Token , this.selectValue)
      if (this.addr2Token && this.selectValue) {
        this.queryMaxLoading = true
        methods.getShortsMoV(this.selectValue, this.addr2Token).call((err, res) => {
          this.queryMaxLoading = false
          if (!err) {
            this.maxAmountShort = (res/Math.pow(10, 18)).toFixed(8);
            console.log('最大做空:', this.maxAmountShort)
          } else {
            this.maxAmountShort = '0.00000000';
          }
        })
      }
    },
    onChangePairIndex (index) {
      this.selectPairIndex = index;
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/pages/index.scss';
.zr0-cls-0 {
animation:zr0-ani-0 0.5s cubic-bezier(0.33,1,0.68,1) 0.5s both;
}
.zr0-cls-1 {
animation:zr0-ani-1 0.5s cubic-bezier(0.33,1,0.68,1) 0.4375s both;
}
.zr0-cls-2 {
animation:zr0-ani-2 0.5s cubic-bezier(0.33,1,0.68,1) 0.375s both;
}
.zr0-cls-3 {
animation:zr0-ani-3 0.5s cubic-bezier(0.33,1,0.68,1) 0.3125s both;
}
.zr0-cls-4 {
animation:zr0-ani-4 0.5s cubic-bezier(0.33,1,0.68,1) 0.25s both;
}
.zr0-cls-5 {
animation:zr0-ani-5 0.5s cubic-bezier(0.33,1,0.68,1) 0.1875s both;
}
.zr0-cls-6 {
animation:zr0-ani-6 0.5s cubic-bezier(0.33,1,0.68,1) 0.125s both;
}
.zr0-cls-7 {
animation:zr0-ani-7 0.5s cubic-bezier(0.33,1,0.68,1) 0.0625s both;
}
@keyframes zr0-ani-0 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-1 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-2 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-3 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-4 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-5 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-6 {
0% {
transform:scale(0,0);
}
100% {

}
}
@keyframes zr0-ani-7 {
0% {
transform:scale(0,0);
}
100% {

}
}

.home-landing-animation-cover {
  position: relative;
  width: 150px;
  height: 150px;
  margin-top: 30px;
}
#play-landing-animation {
  position: absolute;
  top: 54px;
  left: 54px;
  width: 40px;
  height: 40px;
  border-radius: 100%;
  color: #F72C5B;
  cursor: pointer;
  z-index: 100;
  transition: 0.5s cubic-bezier(0.075, 0.82, 0.165, 1) -webkit-transform;
  transition: 0.5s cubic-bezier(0.075, 0.82, 0.165, 1) transform;
  transition: 0.5s cubic-bezier(0.075, 0.82, 0.165, 1) transform, 0.5s cubic-bezier(0.075, 0.82, 0.165, 1) -webkit-transform;
  &:before {
    animation: fx-plyr-play-button 1.5s ease-out infinite;
    border: 4px solid #F72C5B;
    border-radius: 150%;
    box-shadow: 0 0 10px #F72C5B;
    box-sizing: border-box;
    content: "";
    height: 440%;
    left: -170%;
    position: absolute;
    top: -170%;
    width: 440%;
  }
}
@keyframes fx-plyr-play-button {
    0% {
        transform: scale(0.5)
    }

    to {
        opacity: 0
    }
}

</style>
