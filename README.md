Winning data structure is a graph with the following Invariants:
  1) # of Vertices, V, >= 6
  2) All Vertices can only be counted once in the network
  2) All Vertices in the network must be of the same color (Black or White)
  3) Both the Head Vertex and Tail Vertex must be on opposite borders
  4) ONLY the Head Vertex and Tail Vertex can be a Border Vertex
  5) The outgoing Edge, eo, of any Vertex, v, must be in a different direction than
     the incoming Edge, ei, of that same vertex.

Board (8x8 Boolean Array) Invariants
  1) No pieces can can occupy the four corners [(0,0),(0,8),(8,0),(8,8)]
  2) No white pieces can occupy black's goals [(0,1) to (0,7)] && [(8,1) to (8,7)]
  3) No black pieces can occupy white's goals [(1,0) to (7,0)] && [(1,8) to (7,8)]
  4) No piece, p, can be placed in a position, pos, that is currently occupied
  5a) If two pieces of the same color, p1 and p2, are separated by one horizontal
      move, one vertical move or one diagonal move (one horizontal and one vertical
      move), then the third piece, p3, cannot be placed one vertical move, one
      horizontal move or one diagonal move away from either two pieces.
  5b) If two pieces of the same color, p1 and p2, are separated by any pair of
      possible moves ([vertical, vertical],[v,h],[v,d],[h,d],[h,h],etc...)
