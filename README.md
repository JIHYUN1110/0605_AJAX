# 0605_AJAX

    <script>
        $("button").click(function(){
            $.getJSON ('https://dog.ceo/api/breeds/image/random', function(data){
                $("img").attr("src", data.message)
            }); 
        });    
    </script>
    
