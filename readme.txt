#ex) player_policy is MCTSPolicy(player='X')

recom_moves = [(0, 0), (0, 1), (1, 1)]
tar, tree, last_move = player_policy.move(game, recom_moves, saved_trees, saved_last_move, 25)
game.move(*tar) #좌표tar에 착점
print(game)

#arguments.
#(1) game : 현재 바둑판 state
#(2) recommend moves : 추천좌표
#(3) saved_trees : 이전에 저장한 tree
#(4) saved_last_move : 이전에 저장한 last_move
#(5) iternum : 반복횟수

#output
#(1) tar : 좌표(이차원)
#(2) tree : MCTS 결과 tree
#(3) last_move : int 값

#저장해야하는값
#tree
#last_move

#초기값
#saved_trees = {}
#saved_last_move = None
