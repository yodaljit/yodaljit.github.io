<!DOCTYPE html>
<html>
<head>
	<title>RTC</title>
	<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/2.3.0/socket.io.js"></script>
</head>
<body>
	<video width="500" height="500" autoplay="autoplay"></video>
</body>
<script type="text/javascript">
	let socket = io.connect(window.location.origin)
	video = document.querySelector('video')
	navigator.mediaDevices.getUserMedia({'video': true, 'audio': true}).then(function(stream){
		video.srcObject = stream
	})
</script>
</html>
