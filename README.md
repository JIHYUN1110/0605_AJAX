# 0605_AJAX

    <script>
        $("button").click(function(){
            $.getJSON ('https://dog.ceo/api/breeds/image/random', function(data){
                $("img").attr("src", data.message)
            }); 
        });    
    </script>
   
   
  $.getJSON은 서버에서 AJAX를 활용하여 더 용이하고 빠르게 json 데이터를 받아올 수 있도록 하는 함수!
  
  이건 $.ajax 안에서 {datatype: json, url: url, data: data, success: success}를 이미 설정해두고 있는 상태라고 한다.
  
  그래서 $.getJSON 안에 url 명시해주고, json 데이터 불러와서 하고 싶은 것을 써주면 댕댕이 사진이 나온다!
  
