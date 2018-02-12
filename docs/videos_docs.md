# Videos Documentation

## Get Videos

This is an example of how to get videos.

```go
client := helix.NewClient("your-client-id", nil)

resp, err := client.GetVideos(&helix.VideosParams{
    GameID: "21779",
    Period: "month",
    Type:   "highlight",
    Sort:   "views",
    First:  10,
})
if err != nil {
    // handle error
}

fmt.Printf("%+v\n", resp)
```