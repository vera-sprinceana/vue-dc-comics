<template>
    <footer>
        <div class="colum">
            <div class="col-3">
                <ul v-for="(element, index) in menuDcLeft" :key='index'>
                    <h5> {{element.titolo}} </h5>
                    <li >
                        <a href="#">{{element.name}}</a>
                    </li>
                </ul>
            </div>
            <div class="col-3">
                <ul v-for="(element, index) in menuCenter" :key='index'>
                    <h5> {{element.titolo}} </h5>
                    <li >
                       <a href="#">{{element.name}}</a> 
                    </li>
                </ul> 
            </div>
            <div class="col-3">
                <ul v-for="(element, index ) in  menuRight" :key='index'>
                    <h5> {{element.titolo}} </h5>
                    <li >
                        <a href="#">{{element.name}}</a>
                    </li>
                </ul> 
            
            </div>
             <LogoFooterComp/>
        </div>   

    </footer>
   
</template>

<script>
import LogoFooterComp from '../components/LogoFooterComp'
export default {
  name: 'FooterComp1',
  components:{
      LogoFooterComp,
  },
   data() {
    return {
      menuDcLeft:[
          {
              titolo: 'DC COMICS',
              url:'/DCCOMICS'
          },
          {
              name:'Character',
              url:'/Character'
          },
          {
              name:'Comics',
              url:'/Comics'
          },
          {
              name:'Movies',
              url:'/Movies'
          },
          {
              name:'Tv',
              url:'/Tv'
          },
          {
              name:'Games',
              url:'/Games'
          },
          {
              name:'Videos',
              url:'/Videos'
          },
          {
              name:'News',
              url:'/News'
          },
           {
              titolo: 'SHOP',
              url:'/SHOP'
          },
          {
              name:'Shop DC',
              url:'/Shop DC'
          },
          {
              name:'Shop DC Collectibles',
              url:'/Shop DC Collectibles'
          },
          
      ],
      menuCenter:[
           {
              titolo: 'DC',
          },
           {
              name:'Terms Of Use',
              url:'/TermsOfUse'
          },
           {
              name:'Privacy Policy (New)',
              url:'/PrivacyPolicy(New)'
          },
           {
              name:'Ad Choices',
              url:'/AdChoices'
          },
           {
              name:'Advertising',
              url:'/Advertising'
          },
           {
              name:'Jobs',
              url:'/Jobs'
          },
           {
              name:'Subscriptions',
              url:'/Subscriptions'
          },
           {
              name:'Talent Workshops',
              url:'/TalentWorkshops'
          },
           {
              name:'CPSC Certificates',
              url:'/CPSCCertificates'
          },
           {
              name:'Ratings',
              url:'/Ratings'
          },
           {
              name:'Shop Help',
              url:'/ShopHelp'
          },
           {
              name:'Contact Us',
              url:'/ContactUs'
          },
      ],
      menuRight:[ 
           {
              titolo: 'SITES',
          },
        {
            name:'DC',
            url:'/DC'
        },
        {
            name:'MAD Magazine',
            url:'/MADMagazine'
        },
        {
            name:'DC KIds',
            url:'/DCKIds'
        },
        {
            name:'DC Universe',
            url:'/DCUniverse'
        },
        {
            name:'DC Power Visa',
            url:'/DCPowerVisa'
        },
          
      ]
    }

    }
}
</script>

<style scoped lang="scss">
@import '../style/variable.scss';
    .colum{
        display: flex;  
    };
    .col-3{
        width: calc((100% - 300px)/3 );
    };
    ul{
        list-style-type: none; 
        text-align: left;
    };  
    li{
        color:#8b8b8b;
        text-align: left;  
        a{
            text-decoration: none;
            color:#8b8b8b;
            font-size: 0.8em;
        }
    };
     h5{

        color:$color-white;
    };
    
</style>