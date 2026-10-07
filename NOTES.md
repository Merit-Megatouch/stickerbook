# STICKER BOOK (stickerbook)

Status: scaffolded 2026-10-07. Facts: [notes/scaffold.md](notes/scaffold.md).

## Checklist
- [ ] Window size in game.conf matches the largest PNG (notes/scaffold.md)
- [ ] Every symbol in notes/unresolved.txt has a stand-in in src/host/loader_services.cpp
      (`make analyze GAME=stickerbook` until it reports 0)
- [ ] First run: `make run GAME=stickerbook DEBUG=shots` — crash trace + screenshots in notes/shots
- [ ] Paths: `make run GAME=stickerbook DEBUG=files`; engine trace: `mkdir -p data/var/merit/debug/files && touch data/var/merit/debug/files/resource_locator`
- [ ] Reference code: `make decompile GAME=stickerbook`
- [ ] Translations + help text appear (gamedata/translations/stickerbook.utf8)
- [ ] Sound and music play (`DEBUG=sound`)
- [ ] A full game plays through (`DEBUG=profile` to catch stalls and old-malloc bugs)

## Log
<!-- dated notes: what broke, what fixed it -->
