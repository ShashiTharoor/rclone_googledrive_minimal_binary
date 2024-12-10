git clone rclone github repo 

and then 

CGO_ENABLED=0 go build -ldflags="-s"

It should get you most of the way there

Note that if you want to reduce binary size further, comment out backends in backend/all/all.go that you don't need and commands in cmd/all/all.go
