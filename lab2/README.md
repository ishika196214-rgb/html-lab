

Assignment 2 - Pushing and Cloning a Repository

 Aim :
To push commits to a second repository on the same computer and make a copy of it using clone.

 Task 1: Creating a bare repository and adding it as origin
I created an empty (bare) repository named `html-remote` next to `html-lab`. A bare repository has no working files and only stores commits, so it works like a server. I then added it as a remote named `origin`. When I checked the list of remotes, `origin` appeared twice, once for fetch and once for push. This confirmed that the remote was connected correctly.

 Task 2: Pushing commits to origin
I pushed all the commits from the `main` branch of `html-lab` to origin (`html-remote`). The last line of the push output showed `main -> main`, which means the local `main` branch was successfully pushed to the `main` branch of the remote.

 Task 3: Cloning the repository
I cloned `html-remote` into a new folder named `html-copy`. After cloning, no branch was checked out automatically because the HEAD of the bare repository pointed to `master`, while the commits were on `main`. So I switched to the `main` branch manually. After that, the commit history showed these commits:

- `b286b9f` - Add next meeting heading
- `54e8121` - Add home page

 Result
The same commits appear in both `html-lab` and `html-copy`. This shows that the push and clone were both successful.
