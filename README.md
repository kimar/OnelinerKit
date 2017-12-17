# OnelinerKit

## Create text based screensavers for macOS.

![Banner](banner.png)

## Getting Started

To get started just add **OnelinerKit.framework** as a dependency to your *ScreenSaver* project, inherit from `OnelinerView` and override `func fetchOneline` e.g.:

```
class DeveloperExcusesView: OnelinerView {
	override func fetchOneline(_ completion: (String) -> Void) {
		completion("Just this one line, no more…")
	}
}
```

The screensaver will display whatever is invoked as the `String` argument inside the `completion` closure. The `fetchOneline` method will fetched whenever the screensaver thinks it's necessary.

If you're keen to see a reference implementation, just head over to [DeveloperExcuses](https://github.com/kimar/DeveloperExcuses).

## License

MIT

## Created by

[Marcus Kida](https://github.com/kimar)
