# clean-my-audios
You may need superuser privileges if the folder you open cma with needs superuser rights.
This is because cma creates 2 folders in the dir you provide:

- `cma_done`: This is were files kept go. This prevents listening again to the same things
- `cma_delete`: This is were deleted files go. You are asked for confirmation to delete all mp3s in this dir at the end. This is better than deleting then directly, because you can just move back a mp3 into cma_done or into the base dir if you made a mistake

# Roadmap
- Add folders for genre/mood classification, eg

  cma_classes/
    happy
    energetic
    ...

- Add colors
- Improve mp3-playing CLI (too much info rn)
