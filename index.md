<!DOCTYPE html>
<html>
<head>
	<title>RTC</title>
</head>
<body>
	<video width="500" height="500" autoplay="autoplay"></video>
</body>
<script type="text/javascript">
	let socket = new WebSocket("wss://yodaljit.github.io")
	video = document.querySelector('video')
	navigator.mediaDevices.getUserMedia({'video': true, 'audio': true}).then(function(stream){
		video.srcObject = stream
	})
</script>
</html>
