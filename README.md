# Pocket Message Board

By Astra

A scrolling LED sign for any screen: a neon green dot board with big black letters you can read from the street.
Put it on an iPad in a shop window, a phone, or a computer screen.

**Open it:** https://findastra.github.io/pocket-message-board/

## Using it

- **Any screen, either way up.** The letters fill the screen. Turn a phone or iPad and the sign turns with it; drag
  a computer window to any shape and the sign fills it. On a phone with a notch, the letters stay clear of it.
- **Full screen.** Tap (or click) the sign once to go full screen. Tap again to change the message, speed, letter size
  or colors, then tap **Show sign**. On a computer, **F** goes in and out of full screen.
- **iPhone:** Safari has no full screen for pages, so add it to your Home Screen (Share, then **Add to Home Screen**)
  and open it from the new icon: it opens with no browser bars. That works on an iPad too.
- **Keep the screen on:** the sign asks the device to stay awake while it shows, where the browser allows it. For a
  sign that stays up all day, also set the device's auto-lock to never (iPad: Settings → Display & Brightness →
  Auto-Lock → **Never**).

The device remembers the last message, colors, speed and size you set (in that browser only).

## How it was checked

With Platform Platypus's `fit-check` and `device-shots` tools (Mirror Pool,
[findastra/platform-platypus](https://github.com/findastra/platform-platypus)): every phone, iPad and computer window
in its device list, upright and on its side, loaded fresh and turned or resized live. A headless browser pretending to
be a device is not the device: the last check is always the real phone or iPad.

## Files

- `index.html`: the whole sign, with no build step
- `manifest.webmanifest`, `icon-512.png`: Home Screen app name and icon

## Limits

- Full screen needs a browser that allows it for a page (iPad Safari, Android Chrome, computers). iPhone Safari does
  not: use Add to Home Screen.
- Whether the screen stays awake is the browser's call; auto-lock set to never is the sure way.
- Settings are saved in the browser you set them in. Another device, or a cleared browser, starts from "Testing 1, 2, 3".
- The letters are drawn from the device's own bold font, so their exact shapes differ a little between an iPhone,
  Android and Windows.

It was called LED Message Board for its first day; the old link (findastra.github.io/led-message-board) sends you here.
