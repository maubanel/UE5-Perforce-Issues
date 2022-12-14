![](images/line3.png)

### UP5 Perforce Issues

![](images/line3.png)

Here is a list of common issues when using Perforce and Unreal Engine 5

<br>

---


##### `Step 1.`\|`ITL`|:small_blue_diamond:

If you are not logged into a workspace, Unreal will sometimes say source control is connected but it is not conected to any or the correct workspace.  Go to P4V and if you see that there is no workspace log into on.

![make sure you are logged into a workspace](images/noValidWorksspaceP4v.png)

![](images/line2.png)

##### `Step 2.`\|`ITL`|:small_blue_diamond: :small_blue_diamond: 

If you are logged into **P4V** but Unreal is not able to log into perforce.  Make sure that the command line perforce sees that you are registered to a valid port.  Open up **Command Prompt** and make sure that you can connect to the perforce server by typing `p4 info`.  The example below returned a failure to connect.

![p4 port failure](images/p4PortFailure.png)

To connect to the server you need to type `p4 set P4PORT=ssl:helixcore.cct.lsu.edu`.

![p4 set port](images/p4PortSet.png)

Now you should see valid information.  Also confirm that your **Host** (in P4V | Advanced) is the same as the host on your computer using command line (p4 info) listed as your **P4 Host**.  If your command line is wrong, you can reset your host by typing `p4 set P4HOST=HOSTNAME`.

![p4 host](images/CorrectWorkspace.png)

![](images/line2.png)

##### `Step 3.`\|`ITL`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

If you can't loginto your workspace on a given computer you need to make sure that the host is correclty set up.  Compate the **Host** in (P4V | Advanced) with the **P4 Host** listed when running `p4 info` in command line. If your command line is wrong, you can reset your host by typing `p4 set P4HOST=HOSTNAME` or reset the host name in P4V.

![p4 host](images/CorrectWorkspace.png)

![](images/line2.png)

##### `Step 4.`\|`ITL`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Make sure at the end of every work session on any computer that you save all and submit changes from Unreal.  It is also very important to make sure that you have nothing left in your **Pending** list.  This means that it is checked out and will not be available on another computer. Open up **P4V** and make sure your **Pending** list is empty (Open up the window in **View | Pending**. If you do have outstanding items you can press **Submit** in **P4V** and it will submit them and release them for use on your other computer.

![submit stale pending list items](images/addSubmit.png)

![](images/line2.png)

##### `Step 5.`\|`ITL`| :small_orange_diamond:

You should not share **Workspaces** on more than one computer.  Each workspace is based on the machine name.  Also, this would be a sync issue if that other computer has files checked out with saved changes. If you cannot access the workspace because it is from another computer, you will need to create a new workspace. To creat a workspace go to the [Workspace Page](https://github.com/maubanel/p4v-unreal/blob/main/workspaces/README.md#user-content-workspaces-in-p4v).

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 6.`\|`ITL`| :small_orange_diamond: :small_blue_diamond:

The **Perforce Server** is case insensitive so it will see `foo.txt` and `Foo.txt` as the same file.  This is due to Unreal's recommendation to maintain compatibility with their tools. So do not use the same characters in the name of files in the same directory.

![](images/line2.png)

##### `Step 7.`\|`ITL`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

When you quit Unreal make sure you clear your pending list in **P4V**.

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 8.`\|`ITL`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 9.`\|`ITL`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 10.`\|`ITL`| :large_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 11.`\|`ITL`| :large_blue_diamond: :small_blue_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)


##### `Step 12.`\|`ITL`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 13.`\|`ITL`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 14.`\|`ITL`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 15.`\|`ITL`| :large_blue_diamond: :small_orange_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 16.`\|`ITL`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 17.`\|`ITL`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 18.`\|`ITL`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 19.`\|`ITL`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 20.`\|`ITL`| :large_blue_diamond: :large_blue_diamond:

![alt_text](images/.jpg)

![](images/line2.png)

##### `Step 21.`\|`ITL`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt_text](images/.jpg)

![](images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - ADD NEXT TITLE"> -->
![next up next tile](images/banner.png)

![](images/line.png)

| [previous]()| [home](README.md#user-content-ue4-lighting) | [next]()|
|---|---|---|
