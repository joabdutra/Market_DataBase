# Market_DataBase
#-*-coding:UTF-8-*-
from Tkinter import*
class janela:
	def __init__(self,root):

		self.root = root
		fontes2 = ('Times','14')
		fontes =  ('Verdana', '14' )
		
		raiz.title("Gerenciador de estoques") 

		self.b1 = Button(self.root,text='Cadastrar produto')
		self.b1.bind("<Button-1>")
		self.b1.grid(row=1,column=1)

		self.b2 = Button(self.root,text='Deletar produto')
		self.b2.bind("<Button-1>")
		self.b2.grid(row=1,column=2)

		self.b3 = Button(self.root,text='Ver estoque')
		self.b3.bind("<Button-1>")
		self.b3.grid(row=1,column=3)

		self.b4 = Button(self.root,text='Ver medía de vendas')
		self.b4.bind("<Button-1>")
		self.b4.grid(row=1,column=4)







raiz = Tk()
janela(raiz)
raiz.mainloop()
