## Supported boards

Soc | Boards |
|:--|:--|
| Allwinner H2+ | Orange Pi Zero/R1 |
| Allwinner H3 | Orange Pi One/Lite/Pc/PcPlus/Plus/Plus2E/ZeroPlus2 | 
| Allwinner H5 | Orange Pi Pc2/Prime/ZeroPlus/ZeroPlus2| 
| Allwinner H6 | Orange Pi 3/3 LTS/Lite2/OnePlus| 
| Allwinner H616 | Orange Pi Zero2 | 
| Rockchip RK3328 | Orange Pi R1Plus/R1Plus LTS| 
| Rockchip RK3399 | Orange Pi 4/4B | 

## Download links

- 中文链接：     http://www.orangepi.cn
- English link：http://www.orangepi.org

## Build


**build.sh reqires "root" which is dangerous!!!!! LOCAL System WILL be MODIFIED** using 'build.sh docker' does not work.

Instead: Use docker with **debian:10** and use container root user. Current directory is mounted into the container at **/build**.

~~~sh
docker run -it --rm --name orange -v $PWD:/build debian:10 bash
# then within container:
#  > cd /build
#  > ./build.sh
~~~
