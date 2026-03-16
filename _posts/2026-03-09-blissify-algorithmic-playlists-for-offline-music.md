---
layout: post
title: "Blissify: Bringing Algorithmic Playlists to Offline Music Collections"
date: 2026-03-09
---

One thing I genuinely miss from streaming services like Spotify and Apple Music is the algorithmic music discovery. That moment where a track you've never heard before plays and you stop what you're doing to listen. I actually [wrote about how Spotify achieves this on LinkedIn](https://www.linkedin.com/pulse/how-spotify-knows-what-you-want-hear-music-analogies-norris-wiles-yuste/) a while back - the short version is that deep learning neural networks break each track into thousands of tiny time slices, capture the harmonic and timbral fingerprint of each, and then learn patterns in rhythm, texture, energy and mood without anyone defining them upfront. The result is incredibly accurate, seemingly serendipitous music discovery.

When you move to an offline collection running on something like [moOde Audio](https://moodeaudio.org/), you lose all of that. Your library just plays tracks in album order, or shuffles randomly. Random shuffle across 4,000 tracks is... not great. You get jarring jumps from ambient electronica to heavy rock, and it breaks the flow completely.

Enter [blissify](https://github.com/Polochon-street/blissify-rs).

Blissify is an open-source tool that analyses your local music library and creates playlists based on the actual sonic characteristics of each track - tempo, loudness, spectral qualities, tonal features. It uses the [bliss](https://music.metabrainz.org/doc/bliss) library under the hood to compute a "distance" between songs, so given a starting track it can queue up the next song that sounds most similar, creating a smooth, coherent listening session from your own library.

It's essentially the same principle as Spotify's recommendation engine, but running locally against your own files. No cloud, no tracking, no subscription.

I installed it today on the Pi5 that runs my moOde setup and it integrates neatly with MPD (the music player daemon that moOde is built on). After an initial analysis pass across the library, which takes a while but only needs to happen once, you can seed a playlist from any track and let blissify build out a queue of sonically similar music.

It's not as sophisticated as what Spotify does with its billions of data points and collaborative filtering, but for an offline collection it's a genuine game-changer. No more jarring shuffle. Just smooth transitions from one track to the next, chosen by actual audio analysis rather than random chance.

If you run moOde or any MPD-based player and have a local music collection, I'd highly recommend giving [blissify-rs](https://github.com/Polochon-street/blissify-rs) a look.
