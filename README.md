# Click Vibration

## Button er onClick er modhe ai code ta likhun:

```
if(count == 100 || count == 200 || count == 300 || count == 400 ){
Vibrator vibrator = (Vibrator) getSystemService(Context.VIBRATOR_SERVICE);
if (vibrator != null) {
    if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.O) {
        vibrator.vibrate(VibrationEffect.createOneShot(200, VibrationEffect.DEFAULT_AMPLITUDE));
    } else {
        vibrator.vibrate(200);
    }
  }
}
```
