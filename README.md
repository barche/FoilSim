This is a conversion of the FoilSim Java web applet to a pure Java program,
based on the download at [CNET](http://download.cnet.com/FoilSim-3/3000-2054_4-75325174.html)

The original documentation follows below.

# FoilSim

This is a beta 1.4b version of the **FoilSim III** program, and you are
invited to participate in the beta testing. If you find errors in the
program or would like to suggest improvements, please send an e-mail to
Thomas.J.Benson\@nasa.gov.

This page contains an interactive Java applet to explore the various
factors which affect the lift and drag of an airfoil. All of the
information presented by the applet are available within the Beginner\'s
Guide to Aerodynamics. You should start with the slide describing the
factors that affect lift and drag.

## FoilSim III

With this software you can investigate how an aircraft wing produces
lift and drag by changing the values of different factors that produce
aerodynamic forces.

There are several different versions of FoilSim III which require
different levels of experience with the package, knowledge of
aerodynamics, and computer technology. This web page contains the
off-line student version of the program. It includes an off-line user\'s
manual which describes the various options available in the program.
More experienced users can select a [version](Foil.html) of the program
which does not include these instructions and loads faster on your
computer.

## GENERAL INSTRUCTIONS

This program is designed to be interactive, so you have to work with the
program. There are a variety of choices which you must make regarding
the analysis and the display of results. There are two main input
devices used to make a choice, a **push button** or a **drop menu**. To
operate a button, move the cursor over the button and left click with
the mouse. The push buttons occur in groups, and the chosen option is
shown as a **yellow**, \"lighted\" button. The drop down menu has a
descriptive word displayed and an arrow at the right of the box. To make
a choice, left click on the arrow, hold down and drag to make your
selection. The current values of the design variables are presented to
you in boxes. By convention, a white box with black numbers is an input
box and you can change the value of the number. A black box with yellow
numbers is an output box and the value is computed by the program. To
change the value in an input box, select the box by moving the cursor
into the box and clicking the mouse, then backspace over the old number,
enter a new number, then hit the **Enter** key on your keyboard. **You
must hit Enter to send the new value to the program.** For most input
variables you can also use a slider located next to the input box. Click
on the slider bar, hold down and drag the slider bar to change values,
or you can click on the arrows at either end of the slider. At any time,
to return to the original default conditions, click the red **Reset**
button at the upper right of the program.

If you see only a grey box at the top of this page, be sure that Java is
enabled in your browser. If Java is enabled, and you are using the
Windows XP operating system, you need to get a newer version of Java. Go
to this link: <http://www.java.com/en/index.jsp>, try the \"Download It
Now\" button, and then select \"Yes\" when the download box from Sun
pops up.

If you experience difficulties when using the sliders to change
variables, simply click away from the slider and then back to it. If the
arrows on the end of the sliders disappear, click in the areas where the
left and right arrow images should appear, and they should reappear.

## SCREEN LAYOUT

The program screen is divided into four main parts:

1.  On the top left side of the screen is the **View Window**. The view
    window includes a graphic of the airfoil that you are designing and
    several buttons which control the graphic. Details of the window are
    given in the [Graphics](#GRAPHICS) section of this page.
2.  On the upper right side of the screen is the **Control Panel**. The
    control panel holds several push buttons which control the input and
    output to be displayed. Input choices have blue letters and the
    selected input panel appears at the lower left. Output choices have
    red letters and the output panel appears at the lower right. You
    will always see the computed lift, drag, Reynold\'s number and lift
    to drag ratio. You can display lift and drag as numerical values or
    as dimensionless coefficients. Details of the [input
    variables](#INPUT%20VARIABLES) and [output
    variables](#OUTPUT%20VARIABLES) are given below.
3.  On the lower right side of the screen is the **Output Window**. The
    output can be presented as graphs of airfoil performance, a probe
    which you can move through the flowfield, a lift and drag gages, or
    printed numerical values of certain parameters. You select the type
    of output displayed by using the push buttons labeled \"Output:\" on
    the upper right panel.
4.  On the lower left side of the screen is the **Input Window**.
    Various input panels are displayed in this window. You select the
    input panel by using the push buttons labeled \"Input:\" on the
    upper right panel.

## GRAPHICS

The **View Window** contains a schematic drawing of the wing that you
are designing and some buttons to control the schematic drawing.
Possible choices are colored blue while the selected option is colored
yellow.

1.  **Edge** shows the wing as viewed looking along the leading edge.
    The cross section appears as an airfoil or circle with the flow
    going from left to right. You can move the picture within the window
    by moving the cursor into the window, holding down the left mouse
    button, and dragging the airfoil to a new location. You can also
    \"Zoom\" in close to the airfoil by using the green slider at the
    left of the window. If you get lost, pushing the red **Find** button
    will return the airfoil to the initial position.
2.  **Top** shows the wing as viewed from above looking down onto the
    planform. The flow is from bottom to top. Since FoilSim only solves
    for the two-dimensional flow past objects, you won\'t see any flow
    in this view. It is provided only to display the geometry of the
    wing area.
3.  **Side - 3D** shows an orthographic projection of the three
    dimensional wing.
4.  **Moving** shows particles flowing past the airfoil. The particles
    are drawn as line \"traces\". The inclination of the trace is at the
    local flow angle, and the left most part of the trace is the
    particle location. Particles are being periodically released from a
    constant streamwise location upstream of the airfoil.The streamwise
    distance between any two particles is proportional to the local
    velocity.
5.  **Frozen** is a snapshot of the moving particles. In this view, you
    can change the streamwise release point of the particles by moving
    the cursor into the view window, holding down the left mouse, and
    dragging the particles to the left or right. In this view, the
    particles are color coded by the time at which they are released.
    (All of the yellow particles were released at the same streamwise
    location at the same time.)
6.  **Streamlines** are collections of the particle traces to form a
    solid flow line.
7.  **Geometry** shows only the geometry of the wing or airfoil with
    some descriptive labels but with no flow field.

## OUTPUT VARIABLES

There are several different output options available for the **Output
Window** at the lower right. You select the type of output by using the
push buttons on the control panel. The default setting is **Plot** and a
graph will appear in the window. The type of graph is described below
and you can vary the plot by using the **Plot Selection** input panel.
If you display a plot and begin to change the input variables, it may
become necessary to rescale the plot axes by pushing the white
**Rescale** button at the lower left of the window. The types of
available plots are listed below and selcted from an Input Panel.

1.  The default plot is the **Surface Pressure**. The yellow line will
    be a plot of the lower surface pressure, and the magenta line a plot
    of the upper surface pressure. For reference, the green line shows
    the value of free stream pressure.
2.  You may also display the **Surface Velocity**. As with the pressure,
    the yellow line will be a plot of the lower surface, and the magenta
    line a plot of the upper surface.
3.  You may also display the **Drag Polar**. A drag polar is a plot of
    lift coefficient versus drag coefficient for a selected geometry at
    various angles of attack.
4.  The remaining plot choices show **Lift**, **Drag**, **Lift
    Coefficient -Cl**, or **Drag Coefficient - Cd** versus each of the
    input variables. For these plots, the current value of the flow
    conditions is shown as a red dot on the plot.

The **Gages** shows the current value of lift (or lift coefficient) and
drag (or drag coefficient) displayed in scientific notation. The gages
are displayed in the output window and move as the lift and drag are
varied. This display shows the relative sensitivity of lift and drag to
the input variables.

The **Probe** lets you explore the flow around the wing. A probe control
panel appears in the output window when you select \"Probe\" from the
control panel. By default, the probe is turned off. You turn the probe
on by pushing one of the white buttons on the probe panel. The probe
itself will then appear in the view window. You change the location of
the probe using the sliders to the left and below the gauge on the probe
panel. The value of the pressure or the velocity at the location of the
probe tip (magenta ball on the view window) is displayed on the gauge.
Or a green trail of \"smoke\" is swept downstream from the probe
location. You turn the probe off by using the red button located above
the gauge.

The performance options provides a written list of important input and
computed variables in the **Output Window**. You have two options for
performance output; the **Data** option gives the computed lift, drag
and flow conditions, the **Geometry** option shows the coordinates of
the airfoil geometry and the local value of velocity and pressure. These
numbers correspond to the plots of velocity and pressure described
above.

Some additional output from the program is displayed on the control
panel and some input panels. You can choose to display the lift or the
lift coefficient by using the drop menu on the control panel. Similarly,
you can either display the drag or the drag coefficient. The value is
displayed in the output box to the right of the drop menu. Lift and drag
may be expressed in either Imperial (English) or metric units (pounds or
Newtons). On the Flight Test input panel is a group of output boxes that
give the atmospheric conditions of the air. The pressure, temperature,
density, and viscosity will change depending on the altitude and
planetary inputs. On the Size input panel the geometric **aspect ratio**
of the wing is displayed. The aspect ratio is defined to be the square
of the span divided by the wing area and is included in the calculation
of induced drag. The Reynold\'s number is the ratio of inertial forces
to viscous forces and affects the calculated value of the drag
Reynold\'s number and lift to drag ratio are displayed on the control
panel.

## INPUT VARIABLES

The input variables are located on input panels that are displayed at
the lower left. You can select the input to display by using the push
buttons on the control panel. You can choose to vary the Shape, the
Size, or perform a Flight Test of a wing design. You can also display
the Plot Selection Panel and a panel to control the Analysis used in
FoilSim III.

1.  If you choose to **Flight Test**, you can change the value of lift
    by varying the speed, or the altitude. You can flight test your wing
    on the earth (default), on Mars, or in the water by using the choice
    box at the upper right. You can also choose to specify your own
    values of temperature and pressure for air, or to specify your own
    fluid by providing a value of the fluid density.
2.  If you choose **Shape**, you can select a Joukowsky airfoil shape
    (J-foil), an ellipse, or a thin plate cross section by using the
    choice box. You can change the **camber, thickness,** or the **angle
    of attack** of the cross section. The definitions of these geometric
    variables are given on the wing geometry web page. There are some
    push buttons on the airfoil Shape input panel to let you chose some
    \"basic\" airfoil shapes: symmetric airfoil, flat bottom foil,
    negative camber, flat plate, high camber, curved plate, or ellipse.
    Clicking on these buttons will set a representative value of camber,
    thickness, and angle of attack. You can choose to investigate the
    lift created by a rotating cylinder, or a spinning ball. For these
    problems you must specify the **spin rate and radius** and the
    **span** of the cylinder.
3.  If you choose **Size**, you can vary the layout of the wing. You can
    change the **chord, span,** or the wing **area**. The ratio of the
    span to the chord is called the **Aspect Ratio** and this parameter
    has an effect on the lift and drag of the wing. If you have selected
    a cylinder or ball shape, this input panel is not used.
4.  There are a variety of **Analysis** options in FoilSim III. The
    option being used is shown by a yellow lighted button on the
    Analysis panel. You can change the analysis by clicking on a white
    button. The default lift calculation includes a **Stall Model** that
    decreases the lift for angles of attack greater than 10 degrees. The
    option is to use the **Ideal Flow** analysis that neglects viscous
    and compressibility effects. The actual calculations are done with
    ideal flow and the stall model corrects for flow separation at high
    angles of attack. The actual calculation is done for a
    two-dimensional foil. The **Aspect Ratio** correction includes the
    3D wing tip effects on lift. The **Induced Drag** correction
    includes the 3D wing tips effects on drag. The drag is determined by
    a table look-up for experimentally determined values of drag
    coefficient. The values were obtained at a specific Reynold\'s
    number. The **Reynolds number correction** includes the effects of
    changing Reynolds number to the test conditions.

## NEW FEATURES

The NASA Glenn Educational Programs Office will continue to improve and
update FoilSim III based on user input. Changes from previous versions
of the program include:

1.  On **29 Nov 10**, version 1.4b was released. This version corrects a
    graphics problem with the drag coefficient as a function of angle of
    attack, camber, and thickness. And we have corrected a drag
    determination error for negative camber airfoils.
2.  On **23 Nov 10**, version 1.4a was released. In response to a user
    email, we have some basic airfoil shapes available on the airfoil
    \"Shape\" input panel.
3.  On **23 Sep 10**, version 1.3b was released. In response to user
    emails, we have moved the choice button for Imperial or Metric Units
    back to the control panel.
4.  On **27 Jul 10**, version 1.3a was released. This is the first
    release version for FoilSim III and includes drag which was not
    available in FoilSim II. Earlier versions of FoilSim III were
    developmental versions and not released to the public.
