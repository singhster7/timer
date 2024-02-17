function startTimer(duration, display) {
  var timer = duration;
  var minutes, seconds;

  setInterval(function() {
    minutes = parseInt(timer / 60, 10);
    seconds = parseInt(timer % 60, 10);

    minutes = minutes < 10 ? "0" + minutes : minutes;
    seconds = seconds < 10 ? "0" + seconds : seconds;

    display.text(minutes + ":" + seconds);

    if (--timer < 0) {
      timer = duration;
    }
  }, 1000);
}

// Example usage
jQuery(function($) {
  var fiveMinutes = 60 * 5; // 5 minutes in seconds
  var display = $("#time");
  startTimer(fiveMinutes, display);
});
