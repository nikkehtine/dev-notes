[Time on Exercism](https://exercism.org/tracks/go/concepts/time)

A [`Time`](https://golang.org/pkg/time/#Time) in Go is a type describing a moment in time. The date and time information can be accessed, compared, and manipulated through its methods, but there are also some functions called on the `time` package itself. The current date and time can be retrieved through the [`time.Now`](https://golang.org/pkg/time/#Now) function.

## Parsing time

[`time.Parse`](https://golang.org/pkg/time/#Parse)

```go
import "time"

func parseTime() time.Time {
    date := "Tue, 09/22/1995, 13:00"
    layout := "Mon, 01/02/2006, 15:04"

    t, err := time.Parse(layout,date) // time.Time, error
}

// => 1995-09-22 13:00:00 +0000 UTC
```

### Layout

| Time        | Options                                        |
| ----------- | ---------------------------------------------- |
| Year        | 2006 ; 06                                      |
| Month       | Jan ; January ; 01 ; 1                         |
| Day         | 02 ; 2 ; \_2 (For preceding 0)                 |
| Weekday     | Mon ; Monday                                   |
| Hour        | 15 ( 24 hour time format ) ; 3 ; 03 (AM or PM) |
| Minute      | 04 ; 4                                         |
| Second      | 05 ; 5                                         |
| AM/PM Mark  | PM                                             |
| Day of Year | 002 ; \_\_2                                    |
