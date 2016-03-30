# HelloWorld
HelloWorld
import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var message: UILabel!
    let messageArray = ["Addition","comma"]
    var index = 0
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

    @IBAction func dobuttontell(sender: AnyObject) {
        print("button touched")
        let nextString = self.messageArray[index]
        
        self.message.text = nextString
        index++
        index %= self.messageArray.count

}
    
}
