import { LightningElement, track } from "lwc";


export default class App extends LightningElement {
  
  
  @track num1;
  @track num2;
  resultado;


  mudouN1(event){
    this.num1 = Number(event.target.value);
  }

  mudouN2(event){
    this.num2 = Number(event.target.value);
  }

 
  soma(){
    this.resultado = this.num1 + this.num2;
  }

  sub(){
    this.resultado = this.num1 - this.num2;
  }

  div(){
    this.resultado = this.num1 / this.num2;
  }

  mult(){
    this.resultado = this.num1 * this.num2;
  }
}
