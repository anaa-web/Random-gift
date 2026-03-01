<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Quay thưởng</title>

<style>
body{
    text-align:center;
    font-family:Arial;
    margin-top:40px;
}
img{
    width:250px;
    margin-top:20px;
}
button{
    padding:12px 25px;
    font-size:18px;
    cursor:pointer;
}
</style>
</head>

<body>

<h1>🎁 Quay nhận thưởng</h1>

<button onclick="spin()">QUAY NGAY</button>

<br>
<img id="result" src="">

<script>

function spin(){

    let r = Math.random()

    if(r < 0.6){
        document.getElementById("result").src = "voucher.png"
    }
    else{
        let gifts = [
            "qua1.png",
            "qua2.png",
            "qua3.png",
            "qua4.png",
            "qua5.png"
        ]

        let randomGift = gifts[Math.floor(Math.random()*gifts.length)]
        document.getElementById("result").src = randomGift
    }
}

</script>

</body>
</html>
