gameplay.py: test용 code (무시해도 됨)
gamestate.py: 오목 경기 field, 규칙 규정
policies.py: MCTS 구현


# MCTS 사용 법
tar, tree = MCTSPolicy(player='X').move(game, recom_moves, iternum, origin)
origin = copy.deepcopy(tree)


"""
tar: MCTS 결과 좌표 (2차원)
tree: MCTS 결과 트리
X: Player 1
O: Player 2
game: 바둑판 state ('.', 'X', 또는 'O')
recom_moves: CNN추천좌표 ex) [(0,0), (1,0), ... , (11, 11)]
iternum: 반복횟수
origin: 저장해둔 tree 로드
"""
