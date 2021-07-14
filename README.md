- 👋 Hi, I’m @sevilaydemir
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
sevilaydemir/sevilaydemir is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
 # create data points
x = np.linspace(-10, 10, 100)
y = np.linspace(-15, 15, 100)
# create grid
X, Y = np.meshgrid(x, y)
Z = np.sin(X) + np.cos(Y)
# create figure container
fig = plt.figure(figsize=(9, 6))
ax = plt.axes(projection = '3d')
# 3d contour plot
ax.contour3D(X, Y, Z, 100, cmap = 'viridis')
# set labels
ax.set_xlabel('x')
ax.set_ylabel('y')
ax.set_zlabel('z')
# save figure
plt.savefig('3d_contour.png', dpi = 300)
