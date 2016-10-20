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




class janela:
	def __init__(self,root):

		#Definindo frames
		self.root = root
		self.canvas = Canvas(root,width=400,height=400)
		self.canvas.grid(row=8)
		#self.canvas1 = Canvas(root)
		#self.canvas.grid(row=10,column=4)
		fontes2 = ('Times','14')
		fontes =  ('Verdana', '14' )
		
		raiz.title("Gerenciador de estoques") 


		self.msg1 = Label(self.root , text='Insira o codigo de barras:', font=fontes2)
		self.msg1.grid(row=1,columnspan=1,sticky=N)
		#Codigo de barras
		self.Cod = Entry(self.root,width=15,font=fontes)
		self.Cod.focus_force()
		self.Cod.grid(column=1,row=1,sticky=W)

		self.msg2 = Label(self.root , text='Insira a quantidade de peças vendidas no mês:', font=fontes2)
		self.msg2.grid(row=2,sticky=N)
		#Quantidade de peças vendidas no mês
		self.vendidas = Entry(self.root,width=15,font=fontes)
		self.vendidas.focus_force()
		self.vendidas.grid(column=1,row=2, sticky=W)

		self.msg3 = Label(self.root , text='Insira o valor do produto:', font=fontes2)
		self.msg3.grid(row=3,columnspan=1)
		#Valor do produto
		self.valor = Entry(self.root,width=15,font=fontes)
		self.valor.focus_force()
		self.valor.grid(column=1,row=3)


		self.msg4 = Label(self.root , text='Insira a quantidade de peças no estoque:', font=fontes2)
		self.msg4.grid(row=4)
		#quantidade de peças no estoque
		self.valor = Entry(self.root,width=15,font=fontes)
		self.valor.focus_force()
		self.valor.grid(column=1,row=4, sticky=W)



		self.b1 = Button(self.root,text='Cadastrar',bg='deepskyblue'
			,padx=10,command=self.Cadastro)
		self.b1.bind("<Button-1>",self.Cadastro)
		self.b1.grid(column=4,row=5,sticky=W)


		self.msg4 = Label(self.root,text='Aquardando' , font=fontes2)
		self.msg4.grid(row=5)


		self.b2 = Button(self.root,text='Ver estoque',bg='deepskyblue',fg='black')
		self.b2.bind("<Button-1>")
		self.b2.grid(column=8,sticky=W,row=0)

		self.b3 = Button(self.root,text='Ver média de vendas',bg='deepskyblue',fg='black')
		self.b3.bind("<Button-1>")
		self.b3.grid(column=8,sticky=W,row=1)

		


		



	def Cadastro(self,event):
		self.msg4['text']="Cadastrando"
		COD=self.Cod.get()
		VAL=self.Valor.get()
		VEN=self.vendidas.get()

		if COD == VEN:
			C.append(Codigo)
			V.append(valor)
			L.append(vendidas)
			print(C,V,L)
			self.msg4['text'] = 'Produto cadastrado'





raiz = Tk()
janela(raiz)
raiz.mainloop()



















