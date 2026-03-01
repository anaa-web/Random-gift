<!DOCTYPE html>
<html>
<head>
    <title>Random Gift</title>
</head>

<body style="text-align:center; margin-top:100px;">
    <img id="gift" width="300">

<script>
const voucher = "voucher.png"

const otherGifts = [
    "qua1.png",
    "qua2.png",
    "qua3.png",
    "qua4.png",
    "qua5.png"
]

function showRandomGift(){

    let result

    // 60% ra voucher
    if (Math.random() < 0.6){
        result = voucher
    }
    // 40% ra quà khác (random)
    else{
        const i = Math.floor(Math.random() * otherGifts.length)
        result = otherGifts[i]
    }

    document.getElementById("gift").src = result
}

showRandomGift()
</script>

</body>
</html>
