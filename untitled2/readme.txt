# MCTS ����

# tar: MCTS ��� ��ǥ (2����)
# tree: MCTS ��� Ʈ��
# X: Player 1
# O: Player 2
# game: �ٵ��� state ('.', 'X', �Ǵ� 'O')
# recom_moves: CNN��õ��ǥ ex) [(0,0), (1,0), ... , (11, 11)]
# iternum: �ݺ�Ƚ��
# origin: �����ص� tree �ε�

tar, tree = MCTSPolicy(player='X').move(game, recom_moves, iternum, origin)
origin = copy.deepcopy(tree)
