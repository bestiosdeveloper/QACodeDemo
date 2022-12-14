# QACodeDemo
Some helper method to create QR code with logo in center.

![preview](https://github.com/bestiosdeveloper/QACodeDemo/blob/master/DemoImage.png)


## Usage

Code example for setup:

```swift
class ViewController: UIViewController {

@IBOutlet weak var imageView: UIImageView!

override func viewDidLoad() {
super.viewDidLoad()
// Do any additional setup after loading the view.

guard let qrURLImage = URL(string: "https://www.thepramodkumar.com/")?.qrImage(using: #colorLiteral(red: 0.3490196078, green: 0.768627451, blue: 0.6823529412, alpha: 1), logo: #imageLiteral(resourceName: "logo")) else { return }

imageView.image = qrURLImage

}
}
```

## Licence

PKCategoryView is released under the MIT license.
