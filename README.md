# health-safety
class HealthSafety:
    def _init_(self, name, role):
        self.name = name
        self.role = role
        self.safety_score = 100  # Start with a full safety score

    def report_hazard(self, hazard):
        print(f"{self.name} reported a hazard: {hazard}")
        self.safety_score -= 10  # Deduct points for safety risks

    def wear_ppe(self, ppe):
        print(f"{self.name} is wearing {ppe} for protection.")
        self.safety_score += 5  # Increase score for safety compliance

    def follow_procedure(self, procedure):
        print(f"{self.name} is following {procedure}.")
        self.safety_score += 10  # Reward for following procedures

    def emergency_response(self, emergency):
        print(f"Emergency alert: {emergency}! {self.name} is taking action.")
        self.safety_score += 15  # Bonus points for handling emergencies well

    def show_safety_status(self):
        print(f"Safety Score for {self.name}: {self.safety_score}/100")
