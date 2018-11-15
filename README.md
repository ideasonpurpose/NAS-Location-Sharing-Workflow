# Network Drive Location Sharing Automator Workflow
Allows macOS X users in an office to quickly send and open recieved locations on a shared network drive.

All IOP-specific addresses have been removed from this public repository.

## Usage

To share a location, the user selects a file or folder in Finder, and clicks `Services` → `Copy Server Location to Clipboard`. This location can then be pasted into an email, Slack message, or other text based program. It will look like this:

```
💾⌞Office Drive → Jonathan → test → lots → of → folders → Very Important File.mp4⌟💾
```

Users who recieve these locations can highlight them (it's okay to be a bit sloppy), go to the top of the screen, and select `[app name]` (Mail, Slack, Chrome, etc) → `Services` → `Open Location On Server`. 

## Set Up / Installation

Before use, open the workflows in automator, go to the Applescript block, and adjust all lines with a `--change this` comment.

The `share1`, `share2`, and `share3` variables should contain the names of shares in use on your NAS.

The `primaryServerAddress` and `secondaryServerAddress` variables should contain the  address(es) of your NAS. For instance, `primaryServerAddress` might be the server's internal IP address within the office, and `secondaryServerAddress` might be an address that's open to the WAN.

Once set up, copy the Quick Actions to ~/Library/Services/ on any machine or account where they will be used.

## Compatibility

These Quick Actions have been tested on macOS X 10.12 – 10.14, and are likely to work on systems as far back as 10.6.

## About

[![iop_logo](https://cloud.githubusercontent.com/assets/8320/9443542/944a8bce-4a4f-11e5-9d2f-54999b1687d5.png)][iop]  
This project is sponsored by and used in production at [Ideas On Purpose][iop]

[iop]: http://ideasonpurpose.com
