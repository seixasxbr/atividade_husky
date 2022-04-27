# Atividade Husky
Instituição: Universidade Federal da Bahia<br>
Membros: Mateus Seixas, Matheus Soares e Estevão Maciel.
## Para adcionar o ground truth
Adcionar o seguinte trecho de código no arquivo husky.urdf.xacro
```
  <gazebo>
    <plugin name="p3d_base_controller" filename="libgazebo_ros_p3d.so">
      <alwaysOn>true</alwaysOn>
      <updateRate>50.0</updateRate>
      <bodyName>base_link</bodyName>
      <topicName>ground_truth/state</topicName>
      <gaussianNoise>0.01</gaussianNoise>
      <frameName>world</frameName>
      <xyzOffsets>0 0 0</xyzOffsets>
      <rpyOffsets>0 0 0</rpyOffsets>
    </plugin>
  </gazebo>
  ```
  
  ### Bag, CSV's, scrip para plot e plots disponíveis na pasta dados
