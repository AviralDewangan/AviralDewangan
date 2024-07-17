- 👋 Hi, I’m @AviralDewangan
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
// Example Car Movement (Unity C#)
public class CarController : MonoBehaviour {
    public float speed = 10f;
    public float turnSpeed = 200f;

    void Update() {
        float moveForward = Input.GetAxis("Vertical") * speed * Time.deltaTime;
        float turn = Input.GetAxis("Horizontal") * turnSpeed * Time.deltaTime;

        transform.Translate(Vector3.forward * moveForward);
        transform.Rotate(Vector3.up * turn);
    }
}
// Example Collision Handling (Unity C#)
void OnCollisionEnter(Collision collision) {
    if (collision.gameObject.tag == "Obstacle") {
        // Handle collision with obstacle
    }
}
