.. link: 
.. description: 
.. tags: MATE,PulseAudio,GStreamer
.. date: 2012/01/26 00:53:00
.. title: PulseAudio no more required
.. slug: 2012-01-26-pulseaudio-no-more-required
.. author: Stefano Karapetsas

Upgrading to **mate-settings-daemon-1.1.1**, we readded support to gstreamer
(instead of pulseaudio) for media (volume) keys. So, now MATE dont requires
PulseAudio.

Now there are two packages that provides mate-settings-daemon:

  * **mate-settings-daemon-gstreamer** (default): uses gstreamer to provides media keys.
  * **mate-settings-daemon-pulse**: uses pulseaudio to provides media keys.
