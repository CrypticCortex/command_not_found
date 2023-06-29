```sudo chmod -R 775 /usr/local/rvm/gems/default/```

Use this to fix the permissions on the gems folder. This is a known issue with RVM and Docker.

``` ros2 topic error RuntimeError'>:!rclpy.ok()" ```

Fix: 
```bash
ros2 daemon stop
ros2 daemon start
```