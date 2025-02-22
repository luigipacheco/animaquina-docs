=== "Universal Robots"

    !!! note "NOTE"

        This is a pre-alpha version intended for development and testing purposes only. It contains significant limitations and safety risks. Do not use in production environments or without expert supervision.


    # Animaquina  Pre-Alpha for Universal Robots

    ## Version Information
    - Compatible with Blender 4.2
    - Only compatible with Universal Robots (UR) models
    - Requires a startup file for each robot model
    - This is a pre-alpha version and may contain bugs or incomplete features.

    ## Installation

    1. **Use Blender Launcher**: It is advised to use Blender Launcher to keep an isolated version of Blender and Python.
    2. Open Blender 4.2.
    3. Locate your Blender 4.2 Python lib folder. This is typically found in:
    - Windows: `C:\Program Files\Blender Foundation\Blender 4.2\4.2\python\lib`
    - macOS: `/Applications/Blender.app/Contents/Resources/4.2/python/lib`
    - Linux: `/usr/share/blender/4.2/python/lib`
    4. Copy both the URX folder and the math3d folder from the Animaquina download into the Blender Python lib folder.
    5. Go to **Edit** > **Preferences** in Blender.
    6. Click on the **Add-ons** tab.
    7. In the top-right corner of the Add-ons panel, click on **Install**.
    8. Navigate to and select the Animaquina v0.0.3 pre-alpha ZIP file.
    9. Click **Install Add-on**.
    10. Locate "Animaquina" in the add-ons list and enable it by checking the box next to its name.

    ## Usage

    1. Select the robot you have from the drop down list this is either ur16e, ur10e or ur5e
    2. Set the IP address of your Universal Robot in the Animaquina panel.
    3. Click the **Connect** button to establish a connection with the robot.
    4. In the target selection dropdown, select `ur10e_target_twin`.
    5. Click the **Update Pose** button to synchronize the digital twin's TCP with the selected robot's TCP. This action updates the current joint rotation and TCP position of the digital twin robot.
    6. On the info panel, you can view the current joint rotation and TCP position of the digital twin.
    7. To move the robot via Blender:
    a. Manipulate the `ur10e_target_twin` object in the 3D viewport.
    b. Click the **GoTarget** button to send the command and move the physical robot to the new position.
    8. Enable the **RealTime** option to see the digital twin robot moving in sync with the physical robot.
    9. To manually manipulate the physical robot:
    a. Click on **Manual Mode** to enable physical manipulation of the robot.
    b. If **RealTime** is enabled, you will see the robot's movements updated in real-time in the 3D viewport.
    10. To digitize features in the cell:
    a. Move the robot's TCP to the desired position.
    b. Click the **addMarker** button to save the current TCP position as a marker.
    11. To run a toolpath:
        a. Select a mesh object in the 3D viewport.
        b. Click the **Path** button to execute the toolpath.

        !!! warning "warning"
            The order of vertices in the mesh object matters for the toolpath execution. Ensure the vertices are in the correct order before using this function.

    ## Known Issues and Safety Warnings


    !!! warning " **IMPORTANT: USE AT YOUR OWN RISK!** "


        The developer is not responsible for any damage to property, personal injury, or death resulting from the use of this software.

        - **No collision detection:** The software does not detect or prevent collisions between the robot and its environment.
        - **No angle limits:** Joint angle limits are not enforced, which could lead to unexpected or dangerous movements.
        - **Lack of comprehensive safety protocols:** This pre-alpha version does not include industry-standard safety features typically found in production-ready robotic control software.

    ## Additional Safety Precautions

    1. Always maintain a safe distance from the robot during operation.
    2. Use physical safety barriers and emergency stop systems.
    3. Thoroughly test all movements in a controlled, safe environment before executing them on the actual robot.
    4. Ensure that all users are properly trained in robot safety and operation.
    5. Never use this software in production environments or near personnel without proper risk assessment and mitigation strategies.

    For support or to report bugs, please [contact our support team/create an issue on our GitHub repository].


=== "UFactory"

    here be instructions

=== "KUKA"
    coming soon!