# bugzilla
Golnag client for bugzilla API


### list bugs
```go
client, err := bugzilla.NewClient(bugzillaURL, bugzillaUser, bugzillaPassword)
if err != nil {
	return err
}
bugzillaClient.BugList(limit, offset)
```

### bug details for Bug 444
```go
client, err := bugzilla.NewClient(bugzillaURL, bugzillaUser, bugzillaPassword)
if err != nil {
	return err
}
bugzillaClient.BugInfo(444)
```

### add comment to bug 444
```go
client, err := bugzilla.NewClient(bugzillaURL, bugzillaUser, bugzillaPassword)
if err != nil {
	return err
}
client.AddComment(444, "Hello word!"))
```
