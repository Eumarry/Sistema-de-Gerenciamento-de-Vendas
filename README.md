class Venda:
    def __init__(self, id, produto, quantidade, valor_unitario, valor_total):
        self.id = id
        self.produto = produto
        self.quantidade = quantidade
        self.valor_unitario = valor_unitario
        self.valor_total = valor_total
class SistemaDeVendas:
    def __init__(self):
        self.vendas = []

    def registrar_venda(self, venda):
        self.vendas.append(venda)
sistema_de_vendas = SistemaDeVendas()

venda = Venda(1, "Produto A", 2, 10.0, 20)
sistema_de_vendas.registrar_venda(venda)
