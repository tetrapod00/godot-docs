.. _doc_sandbox:

Sandbox
=======

Use roles for editor UI
-----------------------

Adding a sprite and setting some properties
-------------------------------------------

In the :dock:`Scene` dock, click :btn:`2D Scene` to create a new scene.

Add a new :ref:`Sprite2D <class_Sprite2D>` to the scene by right-clicking on the
root node and choosing :btn:`Add Child Node...`. In the :wndw:`Create New Node`
window, search for "Sprite2D", select it, and then click :btn:`Create`.

On the sprite, under :uisection:`Offset`, set :uiproperty:`Offset` to ``(16, 32)``
and enable :uiproperty:`Flip H`. Set :uiproperty:`Animation > HFrames` to ``10``.
In :uisection:`CanvasItem > Visibility`, set the :uiproperty:`Modulate` color to
``ff0000``.

.. tip:: 
    
    Don't forget to save your scene in :path:`Scene > Save Scene...`. When the
    :wndw:`Save Scene As...` window pops up, enter "my_scene.tscn" in the
    :field:`File` field, then click :btn:`Save`.

Setting project settings
------------------------

Go to :path:`Project > Project Settings`, then select the :ref:`Max FPS <class_ProjectSettings_property_application/run/max_fps>`
setting under :projsection:`Application > Run`. Don't forget to click the :btn:`Advanced Settings`
toggle. Then, in :field:`Filter Settings`, search for "physics". Go to
:projsection:`Physics > 3D > Solver`, and set :uiproperty:`Solver Iterations` to ``16``.

All style roles
---------------

Available roles:

- ``:btn:``  A button, toggle, or most other clickable UI elements. 
- ``:field:``  An input field in the editor; anything that you type into. Excludes
  properties, though.
- ``:menu:``  A menu or menu path in the editor. Styled the same as ``:path:``.
- ``:path:``  A UI navigation path in the editor. Includes menu navigation paths,
  or paths like ``Editor > Editor Settings > Shortcuts``, even if the navigation
  path mixes menus and tabs. Use ``:uisection:`` instead for nested sections
  in the inspector. Use ``:uiproperty:`` instead for inspector properties that
  include a section like ``Process > Mode``.
- ``:wndw:``  An editor window, popup dialog, or modal. Anything that can be
  separately dragged and has a title.
- ``:uiproperty:``  A property used in the inspector. Also includes editor settings
  and project settings. 
- ``:uisection:``  A section in the inspector.
- ``:ui:`` - Any other UI. Docks and tabs use this.

Rarely used:

- ``:tab:`` - Tab.
- ``:dock:`` - Dock.
- ``:panel:`` - Panel.
- ``:editor:`` - Any UI in the editor.
- ``:lbl:``  A label in the editor. Anything not clickable.


|styleroles|

.. note::
    
    |styleroles|

.. warning::

    |styleroles|

.. danger::

    |styleroles|

.. tip::

    |styleroles|

.. admonition:: Custom admonition

    |styleroles|

.. All the inline roles which are used in the docs. External links don't work in a substitution.
.. |styleroles| replace:: Built-in styles: ``code``, **bold**, and *italics*.
    Built-in roles: :kbd:`kbd`, :ref:`ref <doc_about_intro>`, :ref:`ref <class_node>`.
    Custom roles: :btn:`btn`, :editor:`editor`, :field:`field`, :lbl:`lbl`,
    :menu:`menu`, :path:`path > path > path`, :ui:`ui`, :uiproperty:`uiproperty`,
    :uisection:`uiproperty`, and :wndw:`wndw`.

