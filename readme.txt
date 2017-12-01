# origin 초기값 : None

# MCTS 수행
# tar : 결과 좌표 (2차원)
# tree: 결과 트리
tar, tree = player_policy.move(game, recom_moves, 2, origin)

# tree 저장
origin = copy.deepcopy(tree)
