# StreamingMediaPlayer
Using native players on iOS and Android.
Testing on iOS 9 and 10 and Android 4.4 and 5 with partial good results.
Works on iOS (tested with the background audio added via https://github.com/aliendb/iosbgaudio) --  but no lock screen controls on 10.  Some lock screen controls on iOS 9. (tray with wrong name at times). 
Android video works with no lock screen controls and won't fail with no background usage. Android audio has an issue.  It breaks due to no background and then it crashes on return to attempt to play again.  Fix for this is to catch for this break in audio. Update applied from original file (SimpleAudioStream.java). 
