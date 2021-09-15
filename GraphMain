import sys
import Project1A_2


if (len(sys.argv)>4):
    n=4
    Project1A_2.build_axis(int(sys.argv[1]),int(sys.argv[2]),int(sys.argv[3]))
    for x in range(4,len(sys.argv)):
        Project1A_2.plot_line(str(sys.argv[x]),n,len(sys.argv),int(sys.argv[1]))
        n+=1
elif(len(sys.argv)>3):
    n=3
    Project1A_2.build_axis(int(sys.argv[1]),int(sys.argv[2]),int(sys.argv[3]))
    f=Project1A_2.input_formulae()
    Project1A_2.plot_line(f,n,len(sys.argv),int(sys.argv[1]))

elif(len(sys.argv)>0):
    n=0
    s=Project1A_2.input_scale()
    Project1A_2.build_axis(int(s[0]),int(s[1]),int(s[2]))
    f=Project1A_2.input_formulae()
    Project1A_2.plot_line(f,n,len(sys.argv),int(s[0]))
    
