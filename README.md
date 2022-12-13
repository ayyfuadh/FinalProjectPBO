# FinalProjectPBO
finalprojectPBO

OOP yang di implementasikan pada Final Project

- Overriding 
 Nama file = Reallmage

    public RealImage(String src) {
        this.src = src;
    }
    @Override
    public ImageIcon loadImage() {
        if(imageIcon == null) {
            this.imageIcon = new ImageIcon(getClass().getResource(src));
        }
        return imageIcon;
    }
    
}

- Encapsulation
Nama file = TubeColumn

public class TubeColumn {

    private int base = Window.HEIGHT - 60;

    private List<Tube> tubes;
    private Random random;
    private int points = 0;
    private int speed = 5;
    private int changeSpeed = speed;

    public TubeColumn() {
        tubes = new ArrayList<>();
        random = new Random();
        initTubes();
    }
    
- Inheritance
Nama file = bird
    
    public class Bird extends GameObject {

    private ProxyImage proxyImage;
    private Tube[] tube;
    public Bird(int x, int y){
    
- Interface
Nama file = IImage
    
    public interface IImage {
    public ImageIcon loadImage();
}

- ArrayList
Nama file = TubeColumn

     public TubeColumn() {
        tubes = new ArrayList<>();
        random = new Random();
        initTubes();

- Generics
Nama file = TubeColumn

public List<Tube> getTubes() {
        return tubes;
    }

    public void setTubes(List<Tube> tubes) {
        this.tubes = tubes;
    
- GUI(graphic user interface)
Nama file = Window
    
    public Window(int width, int height, String title, Game game) {
        JFrame frame = new JFrame();
        frame.add(game);
        frame.setTitle(title);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setMaximumSize(new Dimension(width, height));
        frame.setPreferredSize(new Dimension(width, height));
        frame.setMinimumSize(new Dimension(width, height));
        frame.setLocationRelativeTo(null);
        frame.setResizable(false);
        frame.setVisible(true);
  
Link yt : https://youtu.be/HjCeOnaVFvw

sumber  : https://code-projects.org/flappy-bird-game-in-java-with-source-code/            
