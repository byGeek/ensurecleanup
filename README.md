# ensurecleanup
c++ template class used for RAII

This code is copyed from The book: Windows via c++.


## Demo use
```c++
      // Open the source file without buffering & get its size
      CEnsureCloseFile hFileSrc = CreateFile(pszFileSrc, GENERIC_READ, 
         FILE_SHARE_READ, NULL, OPEN_EXISTING, 
         FILE_FLAG_NO_BUFFERING | FILE_FLAG_OVERLAPPED, NULL);
      if (hFileSrc.IsInvalid()) goto leave;
```
