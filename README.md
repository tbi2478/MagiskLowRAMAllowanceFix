
# Memory Management fix for low memory (Magisk Module)

## This is the basic explanation.

### What's the issue?

The issue is that on lower end devices running low on memory (like mine on 4GB), they automatically try to preserve RAM which is actually low already. So the given Magisk Module fixes it by telling the android device to try and preserve, lesser memory (for me, Default = 1GB).

Specifically, it changes your Free RAM Target from roughly 1GB down to about 100–200MB.

### How it works:
Android uses a property called ro.lmk.thrashing_limit. By default on many high-end ROMs, this is set to 100, which sounds good but actually makes the phone "panic" and start killing background apps (like your music) while you still have a massive 1GB of RAM sitting empty.

### This doesn't affect battery
If you have noticed that your device closes background apps like music apps, OTP apps regular, then it actually increases your battery as your phone doesn;t have to waste it by you reopoening your apps.

I hope this fix helps you, have a good day!!! :3
