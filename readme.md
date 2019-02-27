# check-list

```
- pull server directory
- each file on local directory
  - if file exists on the server :
    - if size changed => mark for upload
    - if date changed => set a warning
  - if file not on server :
    - if close match with remote file name (lowercase, spaces,...) => reject
    - if double-spaces, or extra-dots => reject
    - if other illegal characters "?&()[]:_" => reject
    - if not strict lowercase alpha-numeric => warning
    - if near-collision with another new file => reject both files.
    
- display results and prompt user to continue.  
```
