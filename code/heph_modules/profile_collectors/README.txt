So here's how this interface/implementation system works:

- All the dating platforms (OKC, Tinder, etc.) will have their own implementations of ProfileCollector.
- Every implementation MUST have a method called collect_profile(blacklist_folder_path), that returns a ProfileRawtext
- This ProfileRawtext is used as input for the FaceExtractorServer (see hephmodules/face_extractor/debug_face_extractor_snippets.txt)
