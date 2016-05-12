# Environment:
# /bin/sh
# cwd=/
# run as user
# minimal env (HOME USER LOGNAME fixed-PATH)
# no args

# In other words: ControlPlane seems to basically do:
# clean env ; cd / ; /bin/sh "entire argument that was entered in the prefs box"

# However in the "generic" wrapper we then "exec" the next script (allowing us
# to use any shell), and add basename $0 (allowing us to pass the action as an
# argument).

