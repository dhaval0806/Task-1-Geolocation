# Task-1-Geolocation

<!Doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>get the location</title>
<script>
var id= document.getElementById("Location Implementation");
    function currentposition(){
        if(navigator.geolocation){
            navigator.geolocation.getCurrentPosition(getposition)
        }
        
        else{
            id.innerHTML="geolocation doesnot applicable for your browser";
        }
    }

function getposition(position){

    id.innerHTML= "Latitude cordinate=" + position.coords.latitude + "Longitude coordinate=" +  position.coords.longitude ;
}
</script>
</head>
</html>

