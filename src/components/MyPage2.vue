<template id = "body">
    <div id="myfavor">
            
        <div id="myfavor" class="gallery">
            <table style="margin-bottom: 50px; border-spacing: 10px;">
                <tr>
                    
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure><img alt="logo" src="../assets/food.jpg" width="100%"
                            height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure>
                            <img alt="logo" src="../assets/food1.jpg" width="100%" height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure><img alt="logo" src="../assets/food3.jpg" width="100%"
                            height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                    </tr>
                    
                <tr>
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure><img alt="logo" src="../assets/food.jpg" width="100%"
                            height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure>
                            <img alt="logo" src="../assets/food2.jpg" width="100%" height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                    <td style="width: 250px; height: 250px;">
                        <a href="#">
                        <figure><img alt="logo" src="../assets/food1.jpg" width="100%"
                            height="250px" />
                            <figcaption>정보</figcaption>
                        
                        </figure>
                    </a>
                    </td>
                </tr>
            </table>
        </div>
    </div>


</template>

<script>
export default {
    name: 'SignupForm',
    data() {
        return {
            email: '',
            name: '',
            password: '',
            passwordConfirm: '',
            phone: '',
        };
    },
    methods: {
        submitForm() {
            console.log('dd');
        },
    },
};
</script>

<style scoped>
@import "https://www.w3schools.com/w3css/4/w3.css";


#myfavor {
    width: 800px;
    margin: auto;
}
*{ padding: 0; margin: 0; }



.gallery h3{
  width: 100%; height: 50px;
  line-height: 50px; text-align: center;
}


.gallery a{
  display: block; /* 영역적용위해 사용 */
  width: 100%; height: 100%;

  overflow: hidden; /* 넘어가는 자손을 안보이게 처리 */

  position: relative; /* figcaption의 앱솔루트 기준을 현재 요소로 변경 */
}

.gallery figcaption{
  width: 100%; height: 100%;
  background-color: rgba(0,0,0,0.7);
  color: #fff; text-align: center;
  line-height: 200px;

  position: absolute; /* 기본기준 : body */
  top: 0; left: 0;

  opacity: 0; /* 처음에 안보이게 처리 */

  transition: 0.3s; /* 변화되는 CSS에 시간차를 줌 */
}

/* 테두리 */
.gallery figcaption:after{
  content: ''; /* 비워둠 */
  display: block;
  width: calc(100% - 40px);
  height: calc(100% - 40px);
  border: 1px solid #fff;
  box-sizing: border-box;
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
  margin: auto; /* 기준에서 정가운데 오도록 처리 */
}

.gallery a:hover figcaption, .gallery a:focus figcaption{
  opacity: 1;
}
</style>