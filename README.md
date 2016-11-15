
#App MegaSena
[![Swift](https://img.shields.io/badge/swift-3-orange.svg?style=flat)](https://developer.apple.com/swift/) 

Hello! 

 Simple application to improve their knowledge in developing Swift 3.0

The idea of the app is simple: Generate random numbers in the 1..60 screen

<p align="center">
  <img src="https://github.com/mvalbuquerque/megasena/blob/master/App1.png" width="250"/>
  
  <img src="https://github.com/mvalbuquerque/megasena/blob/master/App2.png" width="250"/>
</p>

Tks, 

@mvalbuquerque


```Swift 

import UIKit

class ViewController: UIViewController {

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

    //Vincula a label a uma textfield
    @IBOutlet weak var txt1: UITextField!
    @IBOutlet weak var txt2: UITextField!
    @IBOutlet weak var txt3: UITextField!
    @IBOutlet weak var txt4: UITextField!
    @IBOutlet weak var txt5: UITextField!
    @IBOutlet weak var txt6: UITextField!
    
    
        //Realiza ação do botão
        @IBAction func gerarNumeros(_ sender: Any) {
        //Exibindo um numero randomico
        let bola1 = arc4random_uniform(60)
        
        //Condição para não mostrar número zero
        if bola1 > 0  {
            txt1.text = String (bola1)
        }
        
        let bola2 = arc4random_uniform(60)
        if bola2 > 0  {
            txt2.text = String (bola2)
        }
        
        let bola3 = arc4random_uniform(60)
        if bola3 > 0 {
            txt3.text = String (bola3)
        }
        
        let bola4 = arc4random_uniform(60)
        if bola4 > 0 {
            txt4.text = String (bola4)
        }
        
        let bola5 = arc4random_uniform(60)
        if bola5 > 0 {
            txt5.text = String (bola5)
        }
        
        let bola6 = arc4random_uniform(60)
        if bola6 > 0 {
            txt6.text = String (bola6)
        }

    }

}

