# clean-my-audios
You may need superuser privileges if the folder you open cma with needs superuser rights.
This is because cma creates 2 folders in the dir you provide:

- `cma_done`: This is were files kept go. This prevents listening again to the same things
- `cma_delete`: This is were deleted files go. You are asked for confirmation to delete all mp3s in this dir at the end. This is better than deleting then directly, because you can just move back a mp3 into cma_done or into the base dir if you made a mistake

# Roadmap
- Add folders for genre/mood classification, eg
```
    cma_classes/
      happy/*.mp3
      energetic/*mp3
      ...
```
- Add colors
- Improve mp3-playing CLI (too much info rn)
- Add option to use "Keep file ?" instead of "Delete that file" for confirmation
- Add usage notice if `$# < 1`
- Add log, eg
```
	DELD: $file
    KEPT: $file
```
(in case `mv` fails, you can do it manually)

- Add progress % of mp3s in cma_done+cma_delete over mp3s in ./
