# Liquidator Audio

Private audio storage for the Liquidator RP server.

92 MP3 tracks in 9 genres. The original 71 radio tracks are preserved; 21 custom ambient tracks were imported byte-for-byte from the server content pack. Half-Life / Half-Life 2 built-in tracks and faction spawn music are excluded. Entropy Zero is included as requested.

The playlist names are the genre labels in `playlists.json`; per-track provenance, measured duration and SHA-256 are recorded in `catalog.json`. Imported files keep their source encoding; the original radio collection is 192 kbps, 44.1 kHz stereo.

This repository requires GitHub authentication. Repository URLs are not public playback URLs. Never distribute GitHub credentials to game clients. Install the files with the game repository radio installer and distribute them through the server content/download system.

| Genre | Tracks | Playlist |
| --- | ---: | --- |
| 팀 마이아 (Tim Maia) | 10 | [M3U8](music/tim_maia/playlist.m3u8) |
| 시티팝 (City Pop) | 13 | [M3U8](music/city_pop/playlist.m3u8) |
| 포가튼/미스터리 (Forgotten) | 4 | [M3U8](music/forgotten/playlist.m3u8) |
| 올드팝 (Old Pop) | 8 | [M3U8](music/oldpop/playlist.m3u8) |
| 두머/포스트펑크 (Doomer) | 19 | [M3U8](music/doomer/playlist.m3u8) |
| 연합 클래식/교향곡 (Union) | 17 | [M3U8](music/union/playlist.m3u8) |
| The Liquidator | 5 | [M3U8](music/the_liquidator/playlist.m3u8) |
| Cruel world we live in | 8 | [M3U8](music/cruel_world/playlist.m3u8) |
| Only You Survived | 8 | [M3U8](music/only_you_survived/playlist.m3u8) |

## Ambient migration — 2026-09-28

The Liquidator (5), Cruel world we live in (8), and Only You Survived (8) are now radio genres. Source: [server content pack](https://steamcommunity.com/sharedfiles/filedetails/?id=3735090249). The source paths are retained as metadata; the new filenames use stable, portable ASCII IDs. The matching server change removes the automatic ambient/spawn player and adds one program for each genre to channel 2 while preserving saved programs.

## Verification — 2026-09-28

All 92 catalog file sizes and SHA-256 hashes were checked. The original 71 catalog entries and files are unchanged. All 21 imported MP3 files passed a complete FFmpeg decode; their bytes also match the server content archive. Actual in-game client downloads and listening still need verification.

## Tracks

| Genre | Title | MP3 |
| --- | --- | --- |
| 팀 마이아 (Tim Maia) | Gostava Tanto De Você | [cxSzri346W0](music/tim_maia/cxSzri346W0.mp3) |
| 팀 마이아 (Tim Maia) | Acenda o farol | [tPp9zkjfj7Q](music/tim_maia/tPp9zkjfj7Q.mp3) |
| 팀 마이아 (Tim Maia) | O Descobridor Dos Sete Mares | [PAUlCK8kuGU](music/tim_maia/PAUlCK8kuGU.mp3) |
| 팀 마이아 (Tim Maia) | Eu Amo Você | [qBBwXuEV4jA](music/tim_maia/qBBwXuEV4jA.mp3) |
| 팀 마이아 (Tim Maia) | Réu Confesso | [p7RCHfW2OOY](music/tim_maia/p7RCHfW2OOY.mp3) |
| 팀 마이아 (Tim Maia) | Azul Da Cor Do Mar | [A9kTV-wpiWk](music/tim_maia/A9kTV-wpiWk.mp3) |
| 팀 마이아 (Tim Maia) | Não Vá | [ZkLWfSLRsNQ](music/tim_maia/ZkLWfSLRsNQ.mp3) |
| 팀 마이아 (Tim Maia) | Bons Momentos | [E4rrbVgsthc](music/tim_maia/E4rrbVgsthc.mp3) |
| 팀 마이아 (Tim Maia) | Se eu lembro faz doer | [u2BBkCr58oI](music/tim_maia/u2BBkCr58oI.mp3) |
| 팀 마이아 (Tim Maia) | Do Leme ao Pontal | [9Q8va-qsE4c](music/tim_maia/9Q8va-qsE4c.mp3) |
| 시티팝 (City Pop) | Yasuha - Flyday Chinatown | [4X7ZvpwBiKA](music/city_pop/4X7ZvpwBiKA.mp3) |
| 시티팝 (City Pop) | 杏里 Anri - Good Bye Boogie Dance | [Rrcs9AoXutw](music/city_pop/Rrcs9AoXutw.mp3) |
| 시티팝 (City Pop) | Tomoko Aran - I'm In Love [Warner Bros. Records] 1983 | [pE2D3LWADFg](music/city_pop/pE2D3LWADFg.mp3) |
| 시티팝 (City Pop) | Tomoko Aran - Midnight Pretenders (subtitled) | [KZyS-ms6-RA](music/city_pop/KZyS-ms6-RA.mp3) |
| 시티팝 (City Pop) | 黄昏のBay City | [aQGvlemqUpE](music/city_pop/aQGvlemqUpE.mp3) |
| 시티팝 (City Pop) | Junko Ohashi (大橋純子) - Telephone Number | [XJWqHmY-g9U](music/city_pop/XJWqHmY-g9U.mp3) |
| 시티팝 (City Pop) | Junko Ohashi - I Love You So | [Q2QUngVGxmE](music/city_pop/Q2QUngVGxmE.mp3) |
| 시티팝 (City Pop) | 【松原みき】Miki Matsubara 'Mayonaka no Door -stay with me'(Music Video) Director's Cut 2022 by TELL SATO | [lags8E4hvow](music/city_pop/lags8E4hvow.mp3) |
| 시티팝 (City Pop) | Anri - Driving My Love | [AIpZ92U_BTE](music/city_pop/AIpZ92U_BTE.mp3) |
| 시티팝 (City Pop) | Toshiki Kadomatsu - If you... | [lHxvQ1wKCuA](music/city_pop/lHxvQ1wKCuA.mp3) |
| 시티팝 (City Pop) | Airport Lady - Toshiki Kadomatsu (1984) | [fLxQtcrzTlA](music/city_pop/fLxQtcrzTlA.mp3) |
| 시티팝 (City Pop) | F・L・Y (1991 Mix) | [A-8fdRq2W9w](music/city_pop/A-8fdRq2W9w.mp3) |
| 시티팝 (City Pop) | BREEZIN' | [M1F5_UzwiY4](music/city_pop/M1F5_UzwiY4.mp3) |
| 포가튼/미스터리 (Forgotten) | Fear & Hunger OST - Eastern Wind | [lAKIbre6neM](music/forgotten/lAKIbre6neM.mp3) |
| 포가튼/미스터리 (Forgotten) | Untitled 2 | [BbTSKh_ANPU](music/forgotten/BbTSKh_ANPU.mp3) |
| 포가튼/미스터리 (Forgotten) | I'm afraid | [-CER-ZoeCGg](music/forgotten/-CER-ZoeCGg.mp3) |
| 포가튼/미스터리 (Forgotten) | Septembar - Ostavi trag - (Audio 1976) HD | [OFSCZgG_Aw0](music/forgotten/OFSCZgG_Aw0.mp3) |
| 올드팝 (Old Pop) | Gipsy Kings - Volare (Official Video) | [qmbx4_TQbkA](music/oldpop/qmbx4_TQbkA.mp3) |
| 올드팝 (Old Pop) | Shakatak With Al Jarreau - Day By Day  (November 1985) | [PVru62O-qhc](music/oldpop/PVru62O-qhc.mp3) |
| 올드팝 (Old Pop) | What You Won't Do for Love | [n9DmdAwUbxc](music/oldpop/n9DmdAwUbxc.mp3) |
| 올드팝 (Old Pop) | Predador de Perereca (1982) | [vRBu_RLBt1A](music/oldpop/vRBu_RLBt1A.mp3) |
| 올드팝 (Old Pop) | Let's Groove | [ltjio4AM2uw](music/oldpop/ltjio4AM2uw.mp3) |
| 올드팝 (Old Pop) | Roça Roça (1983) | [mUb9PM8tSRQ](music/oldpop/mUb9PM8tSRQ.mp3) |
| 올드팝 (Old Pop) | Amiga da Minha Mulher | [BwGZKIx5FN8](music/oldpop/BwGZKIx5FN8.mp3) |
| 올드팝 (Old Pop) | Popotão Grandão (1982) | [9tAgBu6xd6E](music/oldpop/9tAgBu6xd6E.mp3) |
| 두머/포스트펑크 (Doomer) | Mr.Kitty - After Dark (Doomer Wave) | [o7g-XBV8CAE](music/doomer/o7g-XBV8CAE.mp3) |
| 두머/포스트펑크 (Doomer) | HOME - Resonance  Ｄｏｏｍｅｒ Ｗａｖｅ 破滅 | [UQ_LeKjcEFE](music/doomer/UQ_LeKjcEFE.mp3) |
| 두머/포스트펑크 (Doomer) | The Walters - I Love You So (Doomer Wave) | [n1B6cs8WuIw](music/doomer/n1B6cs8WuIw.mp3) |
| 두머/포스트펑크 (Doomer) | somebody that i used to know - Ｄｏｏｍｅｒ Ｗａｖｅ | [65C68DnQfMc](music/doomer/65C68DnQfMc.mp3) |
| 두머/포스트펑크 (Doomer) | Mr.Kitty - Dream Diver (Doomer Wave) | [mFrp7hhgxdc](music/doomer/mFrp7hhgxdc.mp3) |
| 두머/포스트펑크 (Doomer) | Где Фантом? - Стихи (Doomer version) | [65_rrjVV68k](music/doomer/65_rrjVV68k.mp3) |
| 두머/포스트펑크 (Doomer) | Surf Curse - Freaks (Doomer) | [dckyHSxXl24](music/doomer/dckyHSxXl24.mp3) |
| 두머/포스트펑크 (Doomer) | øneheart x reidenshi - snowfall | [LlN8MPS7KQs](music/doomer/LlN8MPS7KQs.mp3) |
| 두머/포스트펑크 (Doomer) | Hotline Miami 2: Wrong Number Soundtrack - The Green Kingdom - 02 Untitled | [Y-Qu_Fk23T4](music/doomer/Y-Qu_Fk23T4.mp3) |
| 두머/포스트펑크 (Doomer) | Hotline Miami 2: Wrong Number Soundtrack - Around | [oZjTGFeBXAY](music/doomer/oZjTGFeBXAY.mp3) |
| 두머/포스트펑크 (Doomer) | DOOMER - He was a good stalker | [GQvsXrUtopc](music/doomer/GQvsXrUtopc.mp3) |
| 두머/포스트펑크 (Doomer) | Losing Tomorrow | [cVp3batAF8A](music/doomer/cVp3batAF8A.mp3) |
| 두머/포스트펑크 (Doomer) | F Song | [0qlvKgm-WXM](music/doomer/0qlvKgm-WXM.mp3) |
| 두머/포스트펑크 (Doomer) | Спокойная ночь | [DiDUIfMk7go](music/doomer/DiDUIfMk7go.mp3) |
| 두머/포스트펑크 (Doomer) | Bernard Herrmann - I Still Can't Sleep - Taxi Driver | [cmDgfzpKw5w](music/doomer/cmDgfzpKw5w.mp3) |
| 두머/포스트펑크 (Doomer) | Pinegrove - Need 2 (official lyric video) | [zE_rK8PX83Q](music/doomer/zE_rK8PX83Q.mp3) |
| 두머/포스트펑크 (Doomer) | billy idol - eyes without a face (slowed & reverb) | [a6u00EcpNcs](music/doomer/a6u00EcpNcs.mp3) |
| 두머/포스트펑크 (Doomer) | Silent Hill 2 OST - Prisonic Fairytale (Slowed + Reverb) | [e1H5373Pmm8](music/doomer/e1H5373Pmm8.mp3) |
| 두머/포스트펑크 (Doomer) | Тоска | [1Gw3ZbXcF00](music/doomer/1Gw3ZbXcF00.mp3) |
| 연합 클래식/교향곡 (Union) | Debussy - Arabesque No.1 and No.2 | [9Fle2CP8gR0](music/union/9Fle2CP8gR0.mp3) |
| 연합 클래식/교향곡 (Union) | Clair De Lune | [WKU8DJzipW4](music/union/WKU8DJzipW4.mp3) |
| 연합 클래식/교향곡 (Union) | Franz Liszt - Liebestraum - Love Dream | [KpOtuoHL45Y](music/union/KpOtuoHL45Y.mp3) |
| 연합 클래식/교향곡 (Union) | Debussy: Rêverie | [9AuzJ2GBCGw](music/union/9AuzJ2GBCGw.mp3) |
| 연합 클래식/교향곡 (Union) | Claude Debussy: The Girl with the Flaxen Hair | [TOxJpPiFe0k](music/union/TOxJpPiFe0k.mp3) |
| 연합 클래식/교향곡 (Union) | Tchaikovsky - Valse Sentimentale | [rUuusqy50yk](music/union/rUuusqy50yk.mp3) |
| 연합 클래식/교향곡 (Union) | Schubert - Serenade | [PXis0PtqdXw](music/union/PXis0PtqdXw.mp3) |
| 연합 클래식/교향곡 (Union) | Schubert - "Ständchen" D957 | [I6Njg1LFxFk](music/union/I6Njg1LFxFk.mp3) |
| 연합 클래식/교향곡 (Union) | Serenata D.957 - Schubert | [Huy791G17Ak](music/union/Huy791G17Ak.mp3) |
| 연합 클래식/교향곡 (Union) | Franz Schubert - Marche Militaire | [PKUPBr0eY6Y](music/union/PKUPBr0eY6Y.mp3) |
| 연합 클래식/교향곡 (Union) | One State Anthem (Red Flood/WE) | [JouWDv9dC0g](music/union/JouWDv9dC0g.mp3) |
| 연합 클래식/교향곡 (Union) | J.S. Bach: Orchestral Suite No. 3 in D Major, BWV 1068: II. Air "on the G String" | [0WKrO4w3QuQ](music/union/0WKrO4w3QuQ.mp3) |
| 연합 클래식/교향곡 (Union) | Toshifumi Hinata-Reflections | [MJenceQ9IEw](music/union/MJenceQ9IEw.mp3) |
| 연합 클래식/교향곡 (Union) | Erik Satie - Gnossienne No.1 | [PLFVGwGQcB0](music/union/PLFVGwGQcB0.mp3) |
| 연합 클래식/교향곡 (Union) | Erik Satie - Gymnopédie No.1 | [S-Xm7s9eGxU](music/union/S-Xm7s9eGxU.mp3) |
| 연합 클래식/교향곡 (Union) | Chopin - Nocturne op.9 No.2 | [9E6b3swbnWg](music/union/9E6b3swbnWg.mp3) |
| 연합 클래식/교향곡 (Union) | Valse | [yT9OSzXJG0A](music/union/yT9OSzXJG0A.mp3) |
| The Liquidator | Entropy Zero | [the_liquidator_entropy_zero](music/the_liquidator/the_liquidator_entropy_zero.mp3) |
| The Liquidator | Garbage | [the_liquidator_garbage](music/the_liquidator/the_liquidator_garbage.mp3) |
| The Liquidator | Lesser Zone Day | [the_liquidator_lesser_zone_day](music/the_liquidator/the_liquidator_lesser_zone_day.mp3) |
| The Liquidator | Mossad | [the_liquidator_mossad](music/the_liquidator/the_liquidator_mossad.mp3) |
| The Liquidator | Wardens | [the_liquidator_wardens](music/the_liquidator/the_liquidator_wardens.mp3) |
| Cruel world we live in | City Ambience (Part 1) | [cruel_world_city_ambience_part_1](music/cruel_world/cruel_world_city_ambience_part_1.mp3) |
| Cruel world we live in | City Ambience (Part 2) | [cruel_world_city_ambience_part_2](music/cruel_world/cruel_world_city_ambience_part_2.mp3) |
| Cruel world we live in | City Ambience (Part 3) | [cruel_world_city_ambience_part_3](music/cruel_world/cruel_world_city_ambience_part_3.mp3) |
| Cruel world we live in | Lullaby Of The Rot | [cruel_world_lullaby_of_the_rot](music/cruel_world/cruel_world_lullaby_of_the_rot.mp3) |
| Cruel world we live in | Path To Survival | [cruel_world_path_to_survival](music/cruel_world/cruel_world_path_to_survival.mp3) |
| Cruel world we live in | Hope May Not Be Lost | [cruel_world_hope_may_not_be_lost](music/cruel_world/cruel_world_hope_may_not_be_lost.mp3) |
| Cruel world we live in | Scum City | [cruel_world_scum_city](music/cruel_world/cruel_world_scum_city.mp3) |
| Cruel world we live in | Unknown Path Ahead | [cruel_world_unknown_path_ahead](music/cruel_world/cruel_world_unknown_path_ahead.mp3) |
| Only You Survived | A Note Unsaid | [only_you_survived_a_note_unsaid](music/only_you_survived/only_you_survived_a_note_unsaid.mp3) |
| Only You Survived | Day 1 | [only_you_survived_day_1](music/only_you_survived/only_you_survived_day_1.mp3) |
| Only You Survived | Gray-Tinged Suburbs | [only_you_survived_gray_tinged_suburbs](music/only_you_survived/only_you_survived_gray_tinged_suburbs.mp3) |
| Only You Survived | Night 1 | [only_you_survived_night_1](music/only_you_survived/only_you_survived_night_1.mp3) |
| Only You Survived | NOWT - The Endless City | [only_you_survived_nowt_the_endless_city](music/only_you_survived/only_you_survived_nowt_the_endless_city.mp3) |
| Only You Survived | Repulsive - Akane'S Regret | [only_you_survived_repulsive_akane_s_regret](music/only_you_survived/only_you_survived_repulsive_akane_s_regret.mp3) |
| Only You Survived | Secret From The River | [only_you_survived_secret_from_the_river](music/only_you_survived/only_you_survived_secret_from_the_river.mp3) |
| Only You Survived | Unworn - A Winter That Kills | [only_you_survived_unworn_a_winter_that_kills](music/only_you_survived/only_you_survived_unworn_a_winter_that_kills.mp3) |
