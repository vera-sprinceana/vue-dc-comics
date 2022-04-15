<template>
    <footer>
        <div class="colum">
            <div class="col-3">
                <ul>
                    <h4>DC COMICS</h4>
                    <li>Character</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>Tv</li>
                    <li>Games</li>
                    <li>Viodes</li>
                    <li>News</li>  
                </ul>
                <ul>
                    <h4>SHOP</h4>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li> 
                </ul> 
            </div>
            <div class="col-3">
                <ul>
                    <h4>DC</h4>
                    <li>Terms Of Use</li>
                    <li>Privacy Policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul> 
            </div>
            <div class="col-3">
                <ul>
                    <h4>SITES</h4>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC KIds</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul> 
            </div>
        </div>   
    </footer>
</template>

<script>
export default {
  name: 'FooterComp1'
}
</script>

<style scoped lang="scss">
@import '../style/variable.scss';
    .colum{
        display: flex;   
    };
    .col-3{
        width:190px;
    }
    ul{
        list-style-type: none; 
        text-align: left;
        h4{
            color:$color-white;
        }
        li{
            color:#8b8b8b;
            padding-bottom: 5px;
            text-align: left;  
        }
    }   
</style>